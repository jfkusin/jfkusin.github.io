---
layout: post
title: Matching DNA strands in PowerShell
tags: [programming, DNA, PowerShell]
comments: true
mathjax: true
author: Julian Kusin
---

## Supply a string length to compare two random DNA sequences 
### Shows you where they match according to AT/GC pairs

```powershell
[int]$seqLength = Read-Host "Enter the length of the DNA sequences: "
[array]$nuctides = "A", "C", "T", "G"
$pointer = @(" ")*$seqLength
$numMatches = 0
function Get-RandNuc { 
    $nuctides[(Get-Random 4)]
}
for ($i=0; $i -lt $seqLength; $i++) {
    [array]$sequence1 += Get-RandNuc
    [array]$sequence2 += Get-RandNuc
}
function Check-Pair {
    param($index)
    $pair = $sequence1[$index] + $sequence2[$index]
    if ($pair -contains "TA" -or ($pair -contains "AT") -or ($pair -contains "CG") -or ($pair -contains "GC")) {
        $global:numMatches++
        $true
    }
    else {
        $false
    }
}
for ($j=0; $j -lt $seqLength; $j++)  {
    if (Check-Pair $j) {
        $pointer[$j] = "^"
    }
}
$sequence1 -join ''
$sequence2 -join ''
$pointer -join ''
Write-Host "Your sequences match $numMatches times"




Clear-Variable sequence1
Clear-Variable sequence2
```

Sample:

![Output](https://lavasum.com/assets/img/DNAscript.png)

I recommend [Idera's PowerShell tutorials](https://blog.idera.com/database-tools/chapter-9-functions/) for instilling the 'PowerShell way' to do things.
Unfortunately it's a hard to navigate through the tutorial. A possible workaround is to navigate via the url. To find Chapter 1 without knowing the full 
url/chapter name, you can just navigate to 'https//<i></i>blog.idera.com/database-tools/chapter-1' and it will bring you to https<i></i>//blog.idera.com/database-tools/chapter-1-the-powershell-console
luckily. 

There is also the classic [*PowerShell in a Month of Lunches*](https://www.manning.com/books/learn-windows-powershell-in-a-month-of-lunches-third-edition).
The third edition is the most polished. 

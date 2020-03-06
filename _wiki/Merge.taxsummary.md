---


title: 'Merge.taxsummary'
---
The [merge.taxsummary](merge.taxsummary) command will merge
\*.tax.summary files.


## Default Settings

The merge.taxsummary command has 2 parameters: input and output. The
input parameter is used to list the .tax.summary files you wish to merge
separated by dashes. The output parameter is used to provide a name for
the resulting merged file.

    mothur > merge.taxsummary(input=final.tax.summary-abrecovery.tax.summary, output=merge.tax.summary)

Here is a sample from final.tax.summary:

    taxlevel    rankID  taxon   daughterlevels  total  F003D000    F003D002    F003D004    F003D006 ...    
    0  0   Root    1   64051   5760    5155    5280    6440    ... 
    1  0.2 Bacteria    9   64051   5760    5155    5280    6440    ... 
    2  0.2.2   "Actinobacteria"    1   392 7   2   1   0   ...
    3  0.2.2.1 Actinobacteria  3   392 7   2   1   0   ...
    4  0.2.2.1.2   Actinomycetales 4   347 1   0   0   0   ...
    5  0.2.2.1.2.2 Actinomycetaceae    1   54  0   0   0   0   ...
    6  0.2.2.1.2.2.2   Actinomyces 0   54  0   0   0   0   ...
    5  0.2.2.1.2.10    Corynebacteriaceae  1   1   1   0   0   0 ...
    6  0.2.2.1.2.10.1  Corynebacterium 0   1   1   0   0   0   ...
    5  0.2.2.1.2.34    Propionibacteriaceae    1   288 0   0   0   0   ...
    6  0.2.2.1.2.34.9  Propionibacterium   0   288 0   0   0   0   ...
    ...

Here is a sample from abrecovery.tax.summary:

    taxlevel    rankID  taxon   daughterlevels  total  A   B   C   
    0  0   Root    1   242 84  84  74  
    1  0.2 Bacteria    6   242 84  84  74  
    2  0.2.2   "Actinobacteria"    1   13  0   13  0   
    3  0.2.2.1 Actinobacteria  1   13  0   13  0   
    4  0.2.2.1.3   Bifidobacteriales   1   13  0   13  0   
    5  0.2.2.1.3.1 Bifidobacteriaceae  1   13  0   13  0   
    6  0.2.2.1.3.1.3   Bifidobacterium 0   13  0   13  0   
    2  0.2.5   "Bacteroidetes" 1   81  38  14  29  
    3  0.2.5.2 "Bacteroidia"   1   81  38  14  29  
    4  0.2.5.2.1   "Bacteroidales" 2   81  38  14  29  
    5  0.2.5.2.1.3 "Porphyromonadaceae"    1   26  1   0   25  
    ...

Here is a sample from merge.tax.summary:

    taxlevel    rankID  taxon   daughterlevels  total  A   B   C   F003D000    F003D002 ...    
    0  0   Root    1   64293   84  84  74  5760    5155    ...
    1  0.1 Bacteria    9   64293   84  84  74  5760    5155    ...
    2  0.1.1   "Actinobacteria"    1   405 0   13  0   7   2   ...
    3  0.1.1.1 Actinobacteria  3   405 0   13  0   7   2   ...
    4  0.1.1.1.1   Actinomycetales 4   347 0   0   0   1   0   ...
    5  0.1.1.1.1.1 Actinomycetaceae    1   54  0   0   0   0   0   ...
    6  0.1.1.1.1.1.1   Actinomyces 0   54  0   0   0   0   0   ...
    5  0.1.1.1.1.2 Corynebacteriaceae  1   1   0   0   0   1   0   ...
    6  0.1.1.1.1.2.1   Corynebacterium 0   1   0   0   0   1   0   ...
    5  0.1.1.1.1.3 Propionibacteriaceae    1   288 0   0   0   0   0   ...
    6  0.1.1.1.1.3.1   Propionibacterium   0   288 0   0   0   0   0   ...
    ...

## Revisions

-   1.30.0 First Introduced

[Category:Commands](Category:Commands)
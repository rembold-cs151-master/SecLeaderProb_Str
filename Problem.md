# Shared Motifs

DNA is comprised of a sequence of base-pairs comprised of adenine (A), cytosine (C), thymine (T) and guanine (G). Certain sequences of base pairs can have biological significance, and thus it can be desirable to identify such sequences (called motifs) in a longer strand of DNA. Understanding which motifs have direct biological significance can be difficult however, and thus it can often be useful to identify what motifs are common amongst a collection of DNA strands.

A **common substring** of a collection of strings is a substring of every member of the collection. We say that a common substring is a **longest common substring** if there does not exist a longer common substring. For example, `"CG"` is a common substring of `"ACGTACGT"` and `"AACCGTATA"`, but it is not as long as possible; in this case, `"CGTA"` is a longest common substring of `"ACGTACGT"` and `"AACCGTATA"`.

Note that the longest common substring is not necessarily unique; for a simple example, `"AA"` and `"CC"` are both longest common substrings of `"AACC"` and `"CCAA"`.

Your task is to take a collection of labeled DNA strands, provided in the form of a JSON file, and write a program that will return the longest common substring between **all** the strands in the JSON file.

Example:
```json
{
    "R1": "GATTACA",
    "R2": "TAGACCA",
    "R3": "ATACA"
}
```
should return
```
"AC"
```

What is the longest common substring between the DNA strands in `full_prob.json`? For ease of checking, how many times does each letter appear in this string?






**Credit:** This problem adapted from the Rosalind Project [here](https://rosalind.info/)

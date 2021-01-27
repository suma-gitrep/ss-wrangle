# ss-wrangle(Bonus challenge)

## SUMA SOMA - Section01

## My Play
[The Taming of the Shrew](http://shakespeare.mit.edu/taming_shrew/full.html)

## Speakers

<strong>Speaker 1</strong>: KATHARINA <br>
<strong>Speaker 1</strong>: GREMIO

## Question

Who speaks more times when compared?

## Answer

KATHARINA speaks 124 times where as GREMIO speaks 91 times. so KATHARINA speaks more times compared to GREMIO.

## Commands

- Command used to find how many times Speaker 1 speaks(KATHARINA):
```
grep -o -i KATHARINA data.txt | wc -l
 ```
- Command used to find how many times Speaker 1 speaks(KATHARINA):
```
 grep -o -i GREMIO data.txt | wc -l
 ```
 - command used to find who speaks more times.
```
 echo $(($(grep -o -i GREMIO data.txt | wc -l) > 
$(grep -o -i KATHARINA data.txt | wc -l) ? $(grep -o -i GREMIO data.txt | wc -l)
 : $(grep -o -i KATHARINA data.txt | wc -l)))
```
- command used to generate result file.
```
echo $(($(grep -o -i GREMIO data.txt | wc -l) > 
$(grep -o -i KATHARINA data.txt | wc -l) ? $(grep -o -i GREMIO data.txt | wc -l)
: $(grep -o -i KATHARINA data.txt | wc -l))) > result.txt
```
## Files

[data.txt](https://github.com/suma-gitrep/ss-wrangle/blob/main/data.txt)
[result.txt](https://github.com/suma-gitrep/ss-wrangle/blob/main/result.txt)






# ss-wrangle
## Bonus challenge


## My Play
[The Taming of the Shrew](http://shakespeare.mit.edu/taming_shrew/full.html)

## Speakers

<strong>Speaker 1</strong>: KATHARINA <br>
<strong>Speaker 1</strong>: GREMIO

## Question

Who speaks more times when compared?

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
## input file

[data.txt]()




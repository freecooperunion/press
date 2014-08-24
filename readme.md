# Free Cooper Union Press Archive

Automatically(ish) generate a folder with json files for every press article about Free Cooper Union, including title, author, word count, excerpt, content, date published, lead image url, and some other fields.

## Get JSON files for each link

1. sign up for api key at http://readability.com
2. open Google Sheet called Free Cooper Press Log
3. paste url column into sublime text
4. select all, break selection into lines, jump to line start
5. paste: `https://readability.com/api/content/v1/parser?token=YOUR-KEY&url=`
6. save file in a folder called /press as urls.txt
7. open terminal and cd to /press
8. run `$ wget -i urls.txt`
9. batch cleanup filenames using automator's rename function
10. batch append .json to filenames using automator

# Casio Calculator Program Convertor
A tool to convert russian text from `UTF-8 Русский текст` to `UTF-8 #E571#E674#E672#E672#E66B#E669#E66A #E673#E665#E66B#E672#E673`
## How to use 
_Note:_ You need a file to convert. 
1. Connect your calculator to PC and press <kbd>F1</kbd> on calculator.
2. Open my program, enter input file, now look at this table

| OS Name     | Output path                                   | Notes                                                        |
| ----------- | --------------------------------------------- | ------------------------------------------------------------ |
|             |                                               | In all paths below, replace Example with the name of your program(must be less than 8 symbols) |
| Windows     | `G:\@MAINMEM\Program\Example.txt`             | Replace G with letter of your drive                          |
| MacOS/Linux | `/path/to/drive/@MAINMEM/Program/Example.txt` | Replace /path/to/drive with path to drive                    |

2\.1\. Enter output path and press Enter.\
3\. Disconnect your calculator. Go to Programs and you will see your programm name. Click Edit and enjoy!
### Example (Windows, CMD)
~~~tex ~~
C:\>cd /d C:\Calculator
C:\Calculator
C:\Calculator>echo Привет мир!>utf8ru.txt
~~~~~~~~~
*Calculator connected as USB Drive, drive letter is G*
~~~tex ~~
C:\Calculator>py casio-converter.py
From:utf8ru.txt
To:G:\@MAINMEM\Program\HW.txt
Converted!
From:
C:\Calculator>
~~~~~~~~~
*Calculator disconnected*\
On calculator, I pressed <kbd>Menu</kbd> then Programs(<kbd>B</kbd>), selected my file and pressed <kbd>Edit (F2)</kbd>, and `Привет мир!` opened.
## Roadmap
- [x] Interactive session, read from files
- [ ] GUI
- [ ] Real converter, not an replacer
  - [ ] Full calcurator symbol table support

# Lab Report 5 (Lab Report 3 Revised with find command)

sources: ChatGPT (Prompts: summarize the find command, what are some options for the find command, \
what does find -name do with examples, what does the find -type type command do, what does the find \
-size n command do, what does the find -maxdepth n command do)

## find command
  
The find command is a Unix/Linux command-line utility used to search for files and directories in a specified location \
based on various criteria such as name, size, type, date modified, and more. The basic syntax of the command is as follows:
` find [path] [expression]`

### find -name

fine -name pattern: \
Searches for files with a specific name or pattern. For example, find . -name "*.txt" searches for all files \
in the current directory and its subdirectories that end with the ".txt" extension. \

```
[cs15lwi23aip@ieng6-201]:written_2:364$ find . -name "*.txt"
./non-fiction/OUP/Abernathy/ch1.txt
./non-fiction/OUP/Abernathy/ch14.txt
./non-fiction/OUP/Abernathy/ch15.txt
./non-fiction/OUP/Abernathy/ch2.txt
./non-fiction/OUP/Abernathy/ch3.txt
./non-fiction/OUP/Abernathy/ch6.txt
./non-fiction/OUP/Abernathy/ch7.txt
./non-fiction/OUP/Abernathy/ch8.txt
./non-fiction/OUP/Abernathy/ch9.txt
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/ch7.txt
./non-fiction/OUP/Castro/chA.txt
./non-fiction/OUP/Castro/chB.txt
./non-fiction/OUP/Castro/chC.txt
./non-fiction/OUP/Castro/chL.txt
./non-fiction/OUP/Castro/chM.txt
./non-fiction/OUP/Castro/chN.txt
./non-fiction/OUP/Castro/chO.txt
./non-fiction/OUP/Castro/chP.txt
./non-fiction/OUP/Castro/chQ.txt
./non-fiction/OUP/Castro/chR.txt
./non-fiction/OUP/Castro/chV.txt
./non-fiction/OUP/Castro/chW.txt
./non-fiction/OUP/Castro/chY.txt
./non-fiction/OUP/Castro/chZ.txt
./non-fiction/OUP/Fletcher/ch1.txt
./non-fiction/OUP/Fletcher/ch10.txt
./non-fiction/OUP/Fletcher/ch2.txt
./non-fiction/OUP/Fletcher/ch5.txt
./non-fiction/OUP/Fletcher/ch6.txt
./non-fiction/OUP/Fletcher/ch9.txt
./non-fiction/OUP/Kauffman/ch1.txt
./non-fiction/OUP/Kauffman/ch10.txt
./non-fiction/OUP/Kauffman/ch3.txt
./non-fiction/OUP/Kauffman/ch4.txt
./non-fiction/OUP/Kauffman/ch5.txt
./non-fiction/OUP/Kauffman/ch6.txt
./non-fiction/OUP/Kauffman/ch7.txt
./non-fiction/OUP/Kauffman/ch8.txt
./non-fiction/OUP/Kauffman/ch9.txt
./non-fiction/OUP/Rybczynski/ch1.txt
./non-fiction/OUP/Rybczynski/ch2.txt
./non-fiction/OUP/Rybczynski/ch3.txt
./travel_guides/berlitz1/HandRHawaii.txt
./travel_guides/berlitz1/HandRHongKong.txt
./travel_guides/berlitz1/HandRIbiza.txt
./travel_guides/berlitz1/HandRIsrael.txt
./travel_guides/berlitz1/HandRIstanbul.txt
./travel_guides/berlitz1/HandRJamaica.txt
./travel_guides/berlitz1/HandRJerusalem.txt
./travel_guides/berlitz1/HandRLakeDistrict.txt
./travel_guides/berlitz1/HandRLasVegas.txt
./travel_guides/berlitz1/HandRLisbon.txt
./travel_guides/berlitz1/HandRLosAngeles.txt
./travel_guides/berlitz1/HandRMadeira.txt
./travel_guides/berlitz1/HandRMadrid.txt
./travel_guides/berlitz1/HandRMallorca.txt
./travel_guides/berlitz1/HistoryDublin.txt
./travel_guides/berlitz1/HistoryEdinburgh.txt
./travel_guides/berlitz1/HistoryEgypt.txt
./travel_guides/berlitz1/HistoryFWI.txt
./travel_guides/berlitz1/HistoryFrance.txt
./travel_guides/berlitz1/HistoryGreek.txt
./travel_guides/berlitz1/HistoryHawaii.txt
./travel_guides/berlitz1/HistoryHongKong.txt
./travel_guides/berlitz1/HistoryIbiza.txt
./travel_guides/berlitz1/HistoryIndia.txt
./travel_guides/berlitz1/HistoryIsrael.txt
./travel_guides/berlitz1/HistoryIstanbul.txt
./travel_guides/berlitz1/HistoryItaly.txt
./travel_guides/berlitz1/HistoryJamaica.txt
./travel_guides/berlitz1/HistoryJapan.txt
./travel_guides/berlitz1/HistoryJerusalem.txt
./travel_guides/berlitz1/HistoryLakeDistrict.txt
./travel_guides/berlitz1/HistoryLasVegas.txt
./travel_guides/berlitz1/HistoryMadeira.txt
./travel_guides/berlitz1/HistoryMadrid.txt
./travel_guides/berlitz1/HistoryMalaysia.txt
./travel_guides/berlitz1/HistoryMallorca.txt
./travel_guides/berlitz1/IntroDublin.txt
./travel_guides/berlitz1/IntroEdinburgh.txt
./travel_guides/berlitz1/IntroEgypt.txt
./travel_guides/berlitz1/IntroFWI.txt
./travel_guides/berlitz1/IntroFrance.txt
./travel_guides/berlitz1/IntroGreek.txt
./travel_guides/berlitz1/IntroHongKong.txt
./travel_guides/berlitz1/IntroIbiza.txt
./travel_guides/berlitz1/IntroIndia.txt
./travel_guides/berlitz1/IntroIsrael.txt
./travel_guides/berlitz1/IntroIstanbul.txt
./travel_guides/berlitz1/IntroItaly.txt
./travel_guides/berlitz1/IntroJamaica.txt
./travel_guides/berlitz1/IntroJapan.txt
./travel_guides/berlitz1/IntroJerusalem.txt
./travel_guides/berlitz1/IntroLakeDistrict.txt
./travel_guides/berlitz1/IntroLasVegas.txt
./travel_guides/berlitz1/IntroLosAngeles.txt
./travel_guides/berlitz1/IntroMadeira.txt
./travel_guides/berlitz1/IntroMadrid.txt
./travel_guides/berlitz1/IntroMalaysia.txt
./travel_guides/berlitz1/IntroMallorca.txt
./travel_guides/berlitz1/JungleMalaysia.txt
./travel_guides/berlitz1/WhatToDublin.txt
./travel_guides/berlitz1/WhatToEdinburgh.txt
./travel_guides/berlitz1/WhatToEgypt.txt
./travel_guides/berlitz1/WhatToFWI.txt
./travel_guides/berlitz1/WhatToFrance.txt
./travel_guides/berlitz1/WhatToGreek.txt
./travel_guides/berlitz1/WhatToHawaii.txt
./travel_guides/berlitz1/WhatToHongKong.txt
./travel_guides/berlitz1/WhatToIbiza.txt
./travel_guides/berlitz1/WhatToIndia.txt
./travel_guides/berlitz1/WhatToIsrael.txt
./travel_guides/berlitz1/WhatToIstanbul.txt
./travel_guides/berlitz1/WhatToItaly.txt
./travel_guides/berlitz1/WhatToJamaica.txt
./travel_guides/berlitz1/WhatToJapan.txt
./travel_guides/berlitz1/WhatToLakeDistrict.txt
./travel_guides/berlitz1/WhatToLasVegas.txt
./travel_guides/berlitz1/WhatToLosAngeles.txt
./travel_guides/berlitz1/WhatToMadeira.txt
./travel_guides/berlitz1/WhatToMalaysia.txt
./travel_guides/berlitz1/WhatToMallorca.txt
./travel_guides/berlitz1/WhereToDublin.txt
./travel_guides/berlitz1/WhereToEdinburgh.txt
./travel_guides/berlitz1/WhereToEgypt.txt
./travel_guides/berlitz1/WhereToFWI.txt
./travel_guides/berlitz1/WhereToFrance.txt
./travel_guides/berlitz1/WhereToGreek.txt
./travel_guides/berlitz1/WhereToHawaii.txt
./travel_guides/berlitz1/WhereToHongKong.txt
./travel_guides/berlitz1/WhereToIbiza.txt
./travel_guides/berlitz1/WhereToIndia.txt
./travel_guides/berlitz1/WhereToIsrael.txt
./travel_guides/berlitz1/WhereToIstanbul.txt
./travel_guides/berlitz1/WhereToItaly.txt
./travel_guides/berlitz1/WhereToJapan.txt
./travel_guides/berlitz1/WhereToJerusalem.txt
./travel_guides/berlitz1/WhereToLakeDistrict.txt
./travel_guides/berlitz1/WhereToLosAngeles.txt
./travel_guides/berlitz1/WhereToMadeira.txt
./travel_guides/berlitz1/WhereToMadrid.txt
./travel_guides/berlitz1/WhereToMalaysia.txt
./travel_guides/berlitz1/WhereToMallorca.txt
./travel_guides/berlitz2/Algarve-History.txt
./travel_guides/berlitz2/Algarve-Intro.txt
./travel_guides/berlitz2/Algarve-WhatToDo.txt
./travel_guides/berlitz2/Algarve-WhereToGo.txt
./travel_guides/berlitz2/Amsterdam-History.txt
./travel_guides/berlitz2/Amsterdam-Intro.txt
./travel_guides/berlitz2/Amsterdam-WhatToDo.txt
./travel_guides/berlitz2/Amsterdam-WhereToGo.txt
./travel_guides/berlitz2/Athens-History.txt
./travel_guides/berlitz2/Athens-Intro.txt
./travel_guides/berlitz2/Athens-WhatToDo.txt
./travel_guides/berlitz2/Athens-WhereToGo.txt
./travel_guides/berlitz2/Bahamas-History.txt
./travel_guides/berlitz2/Bahamas-Intro.txt
./travel_guides/berlitz2/Bahamas-WhatToDo.txt
./travel_guides/berlitz2/Bahamas-WhereToGo.txt
./travel_guides/berlitz2/Bali-History.txt
./travel_guides/berlitz2/Bali-WhatToDo.txt
./travel_guides/berlitz2/Bali-WhereToGo.txt
./travel_guides/berlitz2/Barcelona-History.txt
./travel_guides/berlitz2/Barcelona-WhatToDo.txt
./travel_guides/berlitz2/Barcelona-WhereToGo.txt
./travel_guides/berlitz2/Beijing-History.txt
./travel_guides/berlitz2/Beijing-WhatToDo.txt
./travel_guides/berlitz2/Beijing-WhereToGo.txt
./travel_guides/berlitz2/Berlin-History.txt
./travel_guides/berlitz2/Berlin-WhatToDo.txt
./travel_guides/berlitz2/Berlin-WhereToGo.txt
./travel_guides/berlitz2/Bermuda-WhatToDo.txt
./travel_guides/berlitz2/Bermuda-WhereToGo.txt
./travel_guides/berlitz2/Bermuda-history.txt
./travel_guides/berlitz2/Boston-WhereToGo.txt
./travel_guides/berlitz2/Budapest-History.txt
./travel_guides/berlitz2/Budapest-WhatToDo.txt
./travel_guides/berlitz2/Budapest-WhereoGo.txt
./travel_guides/berlitz2/California-History.txt
./travel_guides/berlitz2/California-WhatToDo.txt
./travel_guides/berlitz2/California-WhereToGo.txt
./travel_guides/berlitz2/Canada-History.txt
./travel_guides/berlitz2/Canada-WhereToGo.txt
./travel_guides/berlitz2/CanaryIslands-History.txt
./travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
./travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
./travel_guides/berlitz2/Cancun-History.txt
./travel_guides/berlitz2/Cancun-WhatToDo.txt
./travel_guides/berlitz2/Cancun-WhereToGo.txt
./travel_guides/berlitz2/China-History.txt
./travel_guides/berlitz2/China-WhatToDo.txt
./travel_guides/berlitz2/China-WhereToGo.txt
./travel_guides/berlitz2/Costa-History.txt
./travel_guides/berlitz2/Costa-WhatToDo.txt
./travel_guides/berlitz2/Costa-WhereToGo.txt
./travel_guides/berlitz2/CostaBlanca-History.txt
./travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
./travel_guides/berlitz2/Crete-History.txt
./travel_guides/berlitz2/Crete-WhatToDo.txt
./travel_guides/berlitz2/Crete-WhereToGo.txt
./travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
./travel_guides/berlitz2/Cuba-History.txt
./travel_guides/berlitz2/Cuba-WhatToDo.txt
./travel_guides/berlitz2/Cuba-WhereToGo.txt
./travel_guides/berlitz2/Nepal-History.txt
./travel_guides/berlitz2/Nepal-WhatToDo.txt
./travel_guides/berlitz2/Nepal-WhereToGo.txt
./travel_guides/berlitz2/NewOrleans-History.txt
./travel_guides/berlitz2/Paris-WhatToDo.txt
./travel_guides/berlitz2/Paris-WhereToGo.txt
./travel_guides/berlitz2/Poland-History.txt
./travel_guides/berlitz2/Poland-WhatToDo.txt
./travel_guides/berlitz2/Portugal-History.txt
./travel_guides/berlitz2/Portugal-WhatToDo.txt
./travel_guides/berlitz2/Portugal-WhereToGo.txt
./travel_guides/berlitz2/PuertoRico-History.txt
./travel_guides/berlitz2/PuertoRico-WhatToDo.txt
./travel_guides/berlitz2/PuertoRico-WhereToGo.txt
./travel_guides/berlitz2/Vallarta-History.txt
./travel_guides/berlitz2/Vallarta-WhatToDo.txt
./travel_guides/berlitz2/Vallarta-WhereToGo.txt
```
  
```
[cs15lwi23aip@ieng6-201]:written_2:372$ find . -name "berlitz*"
./travel_guides/berlitz1
./travel_guides/berlitz2
```
  
### find -type
The find -type type command allows you to search for files based on their type.
  
find . -type d: This command searches for directories in the current directory and its subdirectories.
  
```
[cs15lwi23aip@ieng6-201]:written_2:374$ find . -type d
.
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Berk
./non-fiction/OUP/Castro
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Rybczynski
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```
  
find . -type f: This command searches for regular files (i.e., non-directory files) in the current directory and its subdirectories.

```
[cs15lwi23aip@ieng6-201]:written_2:375$ find . -type f
./non-fiction/OUP/Abernathy/ch1.txt
./non-fiction/OUP/Abernathy/ch14.txt
./non-fiction/OUP/Abernathy/ch15.txt
./non-fiction/OUP/Abernathy/ch2.txt
./non-fiction/OUP/Abernathy/ch3.txt
./non-fiction/OUP/Abernathy/ch6.txt
./non-fiction/OUP/Abernathy/ch7.txt
./non-fiction/OUP/Abernathy/ch8.txt
./non-fiction/OUP/Abernathy/ch9.txt
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Berk/ch1.txt
./non-fiction/OUP/Berk/ch2.txt
./non-fiction/OUP/Berk/ch7.txt
./non-fiction/OUP/Castro/chA.txt
./non-fiction/OUP/Castro/chB.txt
./non-fiction/OUP/Castro/chC.txt
./non-fiction/OUP/Castro/chL.txt
./non-fiction/OUP/Castro/chM.txt
./non-fiction/OUP/Castro/chN.txt
./non-fiction/OUP/Castro/chO.txt
./non-fiction/OUP/Castro/chP.txt
./non-fiction/OUP/Castro/chQ.txt
./non-fiction/OUP/Castro/chR.txt
./non-fiction/OUP/Castro/chV.txt
./non-fiction/OUP/Castro/chW.txt
./non-fiction/OUP/Castro/chY.txt
./non-fiction/OUP/Castro/chZ.txt
./non-fiction/OUP/Fletcher/ch1.txt
./non-fiction/OUP/Fletcher/ch10.txt
./non-fiction/OUP/Fletcher/ch2.txt
./non-fiction/OUP/Fletcher/ch5.txt
./non-fiction/OUP/Fletcher/ch6.txt
./non-fiction/OUP/Fletcher/ch9.txt
./non-fiction/OUP/Kauffman/ch1.txt
./non-fiction/OUP/Kauffman/ch10.txt
./non-fiction/OUP/Kauffman/ch3.txt
./non-fiction/OUP/Kauffman/ch4.txt
./non-fiction/OUP/Kauffman/ch5.txt
./non-fiction/OUP/Kauffman/ch6.txt
./non-fiction/OUP/Kauffman/ch7.txt
./non-fiction/OUP/Kauffman/ch8.txt
./non-fiction/OUP/Kauffman/ch9.txt
./non-fiction/OUP/Rybczynski/ch1.txt
./non-fiction/OUP/Rybczynski/ch2.txt
./non-fiction/OUP/Rybczynski/ch3.txt
./travel_guides/berlitz1/HandRHawaii.txt
./travel_guides/berlitz1/HandRHongKong.txt
./travel_guides/berlitz1/HandRIbiza.txt
./travel_guides/berlitz1/HandRIsrael.txt
./travel_guides/berlitz1/HandRIstanbul.txt
./travel_guides/berlitz1/HandRJamaica.txt
./travel_guides/berlitz1/HandRJerusalem.txt
./travel_guides/berlitz1/HandRLakeDistrict.txt
./travel_guides/berlitz1/HandRLasVegas.txt
./travel_guides/berlitz1/HandRLisbon.txt
./travel_guides/berlitz1/HandRLosAngeles.txt
./travel_guides/berlitz1/HandRMadeira.txt
./travel_guides/berlitz1/HandRMadrid.txt
./travel_guides/berlitz1/HandRMallorca.txt
./travel_guides/berlitz1/HistoryDublin.txt
./travel_guides/berlitz1/HistoryEdinburgh.txt
./travel_guides/berlitz1/HistoryEgypt.txt
./travel_guides/berlitz1/HistoryFWI.txt
./travel_guides/berlitz1/HistoryFrance.txt
./travel_guides/berlitz1/HistoryGreek.txt
./travel_guides/berlitz1/HistoryHawaii.txt
./travel_guides/berlitz1/HistoryHongKong.txt
./travel_guides/berlitz1/HistoryIbiza.txt
./travel_guides/berlitz1/HistoryIndia.txt
./travel_guides/berlitz1/HistoryIsrael.txt
./travel_guides/berlitz1/HistoryIstanbul.txt
./travel_guides/berlitz1/HistoryItaly.txt
./travel_guides/berlitz1/HistoryJamaica.txt
./travel_guides/berlitz1/HistoryJapan.txt
./travel_guides/berlitz1/HistoryJerusalem.txt
./travel_guides/berlitz1/HistoryLakeDistrict.txt
./travel_guides/berlitz1/HistoryLasVegas.txt
./travel_guides/berlitz1/HistoryMadeira.txt
./travel_guides/berlitz1/HistoryMadrid.txt
./travel_guides/berlitz1/HistoryMalaysia.txt
./travel_guides/berlitz1/HistoryMallorca.txt
./travel_guides/berlitz1/IntroDublin.txt
./travel_guides/berlitz1/IntroEdinburgh.txt
./travel_guides/berlitz1/IntroEgypt.txt
./travel_guides/berlitz1/IntroFWI.txt
./travel_guides/berlitz1/IntroFrance.txt
./travel_guides/berlitz1/IntroGreek.txt
./travel_guides/berlitz1/IntroHongKong.txt
./travel_guides/berlitz1/IntroIbiza.txt
./travel_guides/berlitz1/IntroIndia.txt
./travel_guides/berlitz1/IntroIsrael.txt
./travel_guides/berlitz1/IntroIstanbul.txt
./travel_guides/berlitz1/IntroItaly.txt
./travel_guides/berlitz1/IntroJamaica.txt
./travel_guides/berlitz1/IntroJapan.txt
./travel_guides/berlitz1/IntroJerusalem.txt
./travel_guides/berlitz1/IntroLakeDistrict.txt
./travel_guides/berlitz1/IntroLasVegas.txt
./travel_guides/berlitz1/IntroLosAngeles.txt
./travel_guides/berlitz1/IntroMadeira.txt
./travel_guides/berlitz1/IntroMadrid.txt
./travel_guides/berlitz1/IntroMalaysia.txt
./travel_guides/berlitz1/IntroMallorca.txt
./travel_guides/berlitz1/JungleMalaysia.txt
./travel_guides/berlitz1/WhatToDublin.txt
./travel_guides/berlitz1/WhatToEdinburgh.txt
./travel_guides/berlitz1/WhatToEgypt.txt
./travel_guides/berlitz1/WhatToFWI.txt
./travel_guides/berlitz1/WhatToFrance.txt
./travel_guides/berlitz1/WhatToGreek.txt
./travel_guides/berlitz1/WhatToHawaii.txt
./travel_guides/berlitz1/WhatToHongKong.txt
./travel_guides/berlitz1/WhatToIbiza.txt
./travel_guides/berlitz1/WhatToIndia.txt
./travel_guides/berlitz1/WhatToIsrael.txt
./travel_guides/berlitz1/WhatToIstanbul.txt
./travel_guides/berlitz1/WhatToItaly.txt
./travel_guides/berlitz1/WhatToJamaica.txt
./travel_guides/berlitz1/WhatToJapan.txt
./travel_guides/berlitz1/WhatToLakeDistrict.txt
./travel_guides/berlitz1/WhatToLasVegas.txt
./travel_guides/berlitz1/WhatToLosAngeles.txt
./travel_guides/berlitz1/WhatToMadeira.txt
./travel_guides/berlitz1/WhatToMalaysia.txt
./travel_guides/berlitz1/WhatToMallorca.txt
./travel_guides/berlitz1/WhereToDublin.txt
./travel_guides/berlitz1/WhereToEdinburgh.txt
./travel_guides/berlitz1/WhereToEgypt.txt
./travel_guides/berlitz1/WhereToFWI.txt
./travel_guides/berlitz1/WhereToFrance.txt
./travel_guides/berlitz1/WhereToGreek.txt
./travel_guides/berlitz1/WhereToHawaii.txt
./travel_guides/berlitz1/WhereToHongKong.txt
./travel_guides/berlitz1/WhereToIbiza.txt
./travel_guides/berlitz1/WhereToIndia.txt
./travel_guides/berlitz1/WhereToIsrael.txt
./travel_guides/berlitz1/WhereToIstanbul.txt
./travel_guides/berlitz1/WhereToItaly.txt
./travel_guides/berlitz1/WhereToJapan.txt
./travel_guides/berlitz1/WhereToJerusalem.txt
./travel_guides/berlitz1/WhereToLakeDistrict.txt
./travel_guides/berlitz1/WhereToLosAngeles.txt
./travel_guides/berlitz1/WhereToMadeira.txt
./travel_guides/berlitz1/WhereToMadrid.txt
./travel_guides/berlitz1/WhereToMalaysia.txt
./travel_guides/berlitz1/WhereToMallorca.txt
./travel_guides/berlitz2/Algarve-History.txt
./travel_guides/berlitz2/Algarve-Intro.txt
./travel_guides/berlitz2/Algarve-WhatToDo.txt
./travel_guides/berlitz2/Algarve-WhereToGo.txt
./travel_guides/berlitz2/Amsterdam-History.txt
./travel_guides/berlitz2/Amsterdam-Intro.txt
./travel_guides/berlitz2/Amsterdam-WhatToDo.txt
./travel_guides/berlitz2/Amsterdam-WhereToGo.txt
./travel_guides/berlitz2/Athens-History.txt
./travel_guides/berlitz2/Athens-Intro.txt
./travel_guides/berlitz2/Athens-WhatToDo.txt
./travel_guides/berlitz2/Athens-WhereToGo.txt
./travel_guides/berlitz2/Bahamas-History.txt
./travel_guides/berlitz2/Bahamas-Intro.txt
./travel_guides/berlitz2/Bahamas-WhatToDo.txt
./travel_guides/berlitz2/Bahamas-WhereToGo.txt
./travel_guides/berlitz2/Bali-History.txt
./travel_guides/berlitz2/Bali-WhatToDo.txt
./travel_guides/berlitz2/Bali-WhereToGo.txt
./travel_guides/berlitz2/Barcelona-History.txt
./travel_guides/berlitz2/Barcelona-WhatToDo.txt
./travel_guides/berlitz2/Barcelona-WhereToGo.txt
./travel_guides/berlitz2/Beijing-History.txt
./travel_guides/berlitz2/Beijing-WhatToDo.txt
./travel_guides/berlitz2/Beijing-WhereToGo.txt
./travel_guides/berlitz2/Berlin-History.txt
./travel_guides/berlitz2/Berlin-WhatToDo.txt
./travel_guides/berlitz2/Berlin-WhereToGo.txt
./travel_guides/berlitz2/Bermuda-WhatToDo.txt
./travel_guides/berlitz2/Bermuda-WhereToGo.txt
./travel_guides/berlitz2/Bermuda-history.txt
./travel_guides/berlitz2/Boston-WhereToGo.txt
./travel_guides/berlitz2/Budapest-History.txt
./travel_guides/berlitz2/Budapest-WhatToDo.txt
./travel_guides/berlitz2/Budapest-WhereoGo.txt
./travel_guides/berlitz2/California-History.txt
./travel_guides/berlitz2/California-WhatToDo.txt
./travel_guides/berlitz2/California-WhereToGo.txt
./travel_guides/berlitz2/Canada-History.txt
./travel_guides/berlitz2/Canada-WhereToGo.txt
./travel_guides/berlitz2/CanaryIslands-History.txt
./travel_guides/berlitz2/CanaryIslands-WhatToDo.txt
./travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
./travel_guides/berlitz2/Cancun-History.txt
./travel_guides/berlitz2/Cancun-WhatToDo.txt
./travel_guides/berlitz2/Cancun-WhereToGo.txt
./travel_guides/berlitz2/China-History.txt
./travel_guides/berlitz2/China-WhatToDo.txt
./travel_guides/berlitz2/China-WhereToGo.txt
./travel_guides/berlitz2/Costa-History.txt
./travel_guides/berlitz2/Costa-WhatToDo.txt
./travel_guides/berlitz2/Costa-WhereToGo.txt
./travel_guides/berlitz2/CostaBlanca-History.txt
./travel_guides/berlitz2/CostaBlanca-WhatToDo.txt
./travel_guides/berlitz2/Crete-History.txt
./travel_guides/berlitz2/Crete-WhatToDo.txt
./travel_guides/berlitz2/Crete-WhereToGo.txt
./travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
./travel_guides/berlitz2/Cuba-History.txt
./travel_guides/berlitz2/Cuba-WhatToDo.txt
./travel_guides/berlitz2/Cuba-WhereToGo.txt
./travel_guides/berlitz2/Nepal-History.txt
./travel_guides/berlitz2/Nepal-WhatToDo.txt
./travel_guides/berlitz2/Nepal-WhereToGo.txt
./travel_guides/berlitz2/NewOrleans-History.txt
./travel_guides/berlitz2/Paris-WhatToDo.txt
./travel_guides/berlitz2/Paris-WhereToGo.txt
./travel_guides/berlitz2/Poland-History.txt
./travel_guides/berlitz2/Poland-WhatToDo.txt
./travel_guides/berlitz2/Portugal-History.txt
./travel_guides/berlitz2/Portugal-WhatToDo.txt
./travel_guides/berlitz2/Portugal-WhereToGo.txt
./travel_guides/berlitz2/PuertoRico-History.txt
./travel_guides/berlitz2/PuertoRico-WhatToDo.txt
./travel_guides/berlitz2/PuertoRico-WhereToGo.txt
./travel_guides/berlitz2/Vallarta-History.txt
./travel_guides/berlitz2/Vallarta-WhatToDo.txt
./travel_guides/berlitz2/Vallarta-WhereToGo.txt
```
  
### find -size
The find -print command prints the names of the files that are found by the find command. It is the \
default action of the find command, so you don't actually need to include the -print option explicitly \
unless you want to use it in combination with other options.

Examples:
The find -size n command allows you to search for files based on their size. Here are some examples:

find . -size +1M: This command searches for files that are larger than 1 megabyte in the current directory and \
its subdirectories.

find . -size -100k: This command searches for files that are smaller than 100 kilobytes in the current directory \
and its subdirectories.

find /usr/bin -size 10c: This command searches for files in the /usr/bin directory and its subdirectories that are\
exactly 10 bytes in size.

In these examples, + means "larger than", - means "smaller than", and no symbol means "exactly equal to". The n value \
is followed by a size unit, such as k for kilobytes, M for megabytes, c for bytes, etc.

```
[cs15lwi23aip@ieng6-201]:written_2:391$ find . -size -4k 
./travel_guides/berlitz1/HandRHongKong.txt
./travel_guides/berlitz1/HandRIbiza.txt
./travel_guides/berlitz1/HandRIstanbul.txt
./travel_guides/berlitz1/HandRJerusalem.txt
./travel_guides/berlitz1/HandRLakeDistrict.txt
./travel_guides/berlitz1/HandRLasVegas.txt
./travel_guides/berlitz1/HandRLisbon.txt
./travel_guides/berlitz1/HandRLosAngeles.txt
./travel_guides/berlitz1/HandRMadeira.txt
./travel_guides/berlitz1/HandRMallorca.txt
./travel_guides/berlitz1/WhatToFrance.txt
./travel_guides/berlitz1/WhatToHawaii.txt
./travel_guides/berlitz1/WhereToHawaii.txt
```

```
[cs15lwi23aip@ieng6-201]:written_2:392$ find . -size +100k
./non-fiction/OUP/Berk/CH4.txt
./non-fiction/OUP/Berk/ch2.txt
./travel_guides/berlitz1/WhereToFrance.txt
./travel_guides/berlitz1/WhereToIndia.txt
./travel_guides/berlitz1/WhereToItaly.txt
./travel_guides/berlitz1/WhereToJapan.txt
./travel_guides/berlitz1/WhereToMalaysia.txt
./travel_guides/berlitz2/Canada-WhereToGo.txt
./travel_guides/berlitz2/China-WhereToGo.txt
./travel_guides/berlitz2/Portugal-WhereToGo.txt
```
  
### find -maxdepth n
The find -maxdepth n command limits the depth of the search to n levels of subdirectories. Here are some examples:

find . -maxdepth 1 -type f: This command searches for all regular files in the current directory, but not in its subdirectories.

find /home -maxdepth 2 -type d -name "Documents": This command searches for all directories named "Documents" that are \
located no more than 2 levels deep in the /home directory tree.

find /usr/share -maxdepth 3 -type f -iname "*.png": This command searches for all files with a ".png" extension that \
are located no more than 3 levels deep in the /usr/share directory tree.

By default, find searches through all subdirectories of the starting directory, but this can be time-consuming and \
may return more results than needed. The -maxdepth option allows you to limit the search to a specific number of levels\
deep, which can save time and help you find files more efficiently.

```
[cs15lwi23aip@ieng6-201]:written_2:394$ find . -maxdepth 1 -type d
.
./non-fiction
./travel_guides
```
  
```
[cs15lwi23aip@ieng6-201]:written_2:395$ find . -maxdepth 2 -type d
.
./non-fiction
./non-fiction/OUP
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```

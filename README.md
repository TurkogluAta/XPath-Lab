# XPath-Lab


The names of all modules on the timetables

    //slot[not(subject = following::slot/subject)]/subject/text()
   
The name, day, time, and room of all lab classes

    //slot[@type='lab']

The details of any module which has more than one lecture in a week
    
    //slot[@type='lecture']/subject[not(. = preceding::slot[@type='lecture']/subject)]/text()

The name of all modules which have classes on Monday
    
    //day[@name = 'monday']/slot/subject/text()

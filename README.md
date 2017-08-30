# TrackRussianPost
libraries is Russian Post api

The library is designed to obtain data on the track code of the Russian post. 
Features: 

russianspost poc = new russianspost(); //initialize the 

poc.mss = 1-6; //Select the operating mode (right display) 

poc.connect(string login, string password, string trackcode) //connect to the server (the username and password from the api tracking mail (https://tracking.pochta.ru/) you need to register) 
disconnect(); //disable 

getdata(); //get encoded data 

getdata(string text); //decrypt string text. Returns an array with numbers from 0 to 8, the value can also accept poc.barcode poc.statys poc.indexpoluk poc.namepoluk poc.typeot poc.massa poc.ot poc.dod




Erstellen in OC: 

    oc new-project dotnet
    oc project dotnet  
    oc new-app openshift/dotnet~https://github.com/rschumm/hallodotnet.git


Erstelle eine Route zum generierten Service - und die App sollte erreichbar sein. 


alles wieder loswerden:  

    oc delete all --selector app=hallodotnet


Doku:   
https://docs.openshift.com/online/using_images/s2i_images/dot_net_core.html

    

Die Beispiel-Applikation wurde mit den dotnet-Tools generiert:  


    dotnet new web 
    dotnet build 
    dotnet run 

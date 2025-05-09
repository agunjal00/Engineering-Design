
# Lab 9

The purpose of this lab is to visualize YANG data models using Pyang and PlantUML. First I installed Pyang and PlantUML.
![App Screenshot]()
I created a new directory and copied the YANG file into the working directory using the following commands
```
mkdir ~/demo
cp ~/iot/lesson9/intrusiondetection.yang ~/demo
cd ~/demo
```
I ran cat intrusiondetection.yang to display the contents of the file in the terminal
## cat intrusiondetection.yang
![App Screenshot]()

I then generated a YIN version of the YANG model using the following command. YIN is an XML-based equivalent of YANG which is easier for machines to parse.
```
pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
```
I ran cat intrusiondetection.yin to display the contents of the XML formatted file.
## cat intrusiondetection.yin 
![App Screenshot]()

I ran the following commands to generate UML representation, view the UML text, and generate the UML diagram: 
```
pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
cat intrusiondetection.uml
python3 -m plantuml intrusiondetection.uml
```
This was the png image generated in my lesson 9 folder showing the structure of the YANG model.
![App Screenshot]()
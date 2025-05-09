
# Lab 9

The purpose of this lab is to visualize YANG data models using Pyang and PlantUML. First I installed Pyang and PlantUML.
![App Screenshot](https://github.com/user-attachments/assets/46d1b0e9-2fa4-4e35-be55-32fcea5b89bb)
I created a new directory and copied the YANG file into the working directory using the following commands
```
mkdir ~/demo
cp ~/iot/lesson9/intrusiondetection.yang ~/demo
cd ~/demo
```
I ran cat intrusiondetection.yang to display the contents of the file in the terminal
## cat intrusiondetection.yang
![App Screenshot](https://github.com/user-attachments/assets/8b35f8a2-c882-4fbe-aecf-e18a07812a47)

I then generated a YIN version of the YANG model using the following command. YIN is an XML-based equivalent of YANG which is easier for machines to parse.
```
pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
```
I ran cat intrusiondetection.yin to display the contents of the XML formatted file.
## cat intrusiondetection.yin 
![App Screenshot](https://github.com/user-attachments/assets/2dced473-ac58-4bcb-b667-1d8425dc8c33)

I ran the following commands to generate UML representation, view the UML text, and generate the UML diagram: 
```
pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
cat intrusiondetection.uml
python3 -m plantuml intrusiondetection.uml
```
This was the png image generated in my lesson 9 folder showing the structure of the YANG model.

![App Screenshot](https://github.com/user-attachments/assets/39bd6467-a293-4ab8-944d-dbd4211c4574)

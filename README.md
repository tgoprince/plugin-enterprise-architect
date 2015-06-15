# ontouml-mdg-ea

http://www.sparxsystems.com/enterprise_architect_user_guide/10/extending_uml_models/introduction_2.html
http://www.sparxsystems.com/enterprise_architect_user_guide/10/extending_uml_models/mdgtechnologies_2.html

We have used MDG technology SDK in EA, a way of profiling UML through EA's interface. 
Each EAP project generates a respective XML file that will be linked together to form the MDG file. 
There is an EAP project for profiling respectively: 
   - the UML diagram (/input/diagram.eap)
   - the UML toolbox (/input/tolbox.eap)
   - the UML language (/input/profile.eap)
   - the UML patterns (/input/pattern.eap)

If you modify one of the EAP projects, you need to generate again their respective(s) XML file(s) of:
   - the UML diagram (/output/diagram/diagram.xml)
   - the UML toolbox (/output/diagram/toolbox.xml)
   - the UML language (/output/diagram/profile.xml)
   - the UML patterns (/output/pattern/)
      - category.xml, mixin.xml, phasepartition.xml, relator.xml, rolemixin.xml, rolepartition.xml, subkindpartition.xml

Then, with the MTS file "profile-mts" you can generate the MDG file (/mdg/ontouml_2_0_technology.xml).

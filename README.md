# OntoUML2.0 EA Plugin

**User Guide: Installation**

Close EA (if opened)
Move "ontouml_2_0_model_template.xml" to "Sparx Systems\EA\ModelPatterns\"
Move "ontouml_2_0_technology.xml" to "Sparx Systems\EA\MDGTechnologies\"
That's it. Now you can just start EA and use the plugin.

**Developer Guide: How we developed the plugin**

We have used MDG technology SDK in EA, a way of profiling UML through EA's interface. Each EAP project below is going to generate a respective XML file. All XML files are later on linked together to form the final plugin file (i.e. ontouml_2_0_technology.xml)

These are the EAP projects for profiling respectively: 
   - UML diagram (/input/diagram.eap)
   - UML toolbox (/input/tolbox.eap)
   - UML language (/input/profile.eap)
   - UML patterns (/input/pattern.eap)

Note: If you modify any EAP project, you will need to generate again their respective(s) XML file(s). These are found at:
   - UML diagram (/output/diagram/diagram.xml)
   - UML toolbox (/output/diagram/toolbox.xml)
   - UML language (/output/diagram/profile.xml)
   - UML patterns (/output/pattern/)
     (category.xml, mixin.xml, phasepartition.xml, relator.xml, rolemixin.xml, rolepartition.xml, subkindpartition.xml)

### mhus-lib changes 3.3

The following changes will be done to switch from version 3.2.x to 3.3.x

- Because the bundles mhu-lib-form and mhu-lib-logging  have no special dependencies the bundles will be merged into the main bundle mhu-lib-core. All pachages will be the same. Also there is no dependency break but the bundles will no more be found in old projects.
- A compleately new implementation of forms and vaadin forms are done. The package changes from demhus.lib.form2 back to de.mhus.lib.form. The definition helper classes (FmText ...) wil not change expecht the FmDefaultSource will be removed because the new forms have no source definition any more. More datails later.
- The MBase concept will be removed. The concept of changing static references will be removed inside the MObject. It will live in MSingleton.get().getBaseControl() any more but not bound on every MObject.
- The project mhus-osgi-tools will become a synchrone minor version number. mhus-osgi-tools:1.3.x will be compatibte with mhus-lib:3.3.x. This means mhus-osgi-tools will become more usage of mhus-lib in the future.
- mhu-lib-framework will be mhu-lib-standalone. It is used for standalone applications or servers and will be named like this.
- The central configuration must be separated to the config object model. For this the central configuration will be named 'Cfg'. also the classes and package will be named 'cfg'. This caused not much trouble because the classes are not used often but will in the future, see next point
- The central configuration can be extended with other configuration sources. Now it's possible not only have confiruartion in the central mhu-config.properties. Now mutable confiuration parameters (CfgString, CfgProperties) can also be bound to other sources or, e.g. dynamic sources.

#### Forms

The forms engine are compleately rewritten and is number 3 now. The old implementation was removed.

- The new forms (3) implementation brings model and implementation more together. Other then in the last implementation (2) there is no separate datasource between the model and the UI. The model can access the UI Classes directly.
- There can be a Control Object to organize the behavior of the form UI. The control will receive events if values are changed.
- The UI elements are loaded by a ComponentAdapter. Adapters will be provided by a ComponentAdapterProvider.
- The reference implementation are the vaadin implementation in mhu-lib-vaadin.
- The vaadin ListEditors are using the new forms engine. There is also a default pojo implementation.
- The default Components are Text, TextArea, Password, RichText, Checkbox, Number and Combobox.
- The default Layouts/Composits are 100 and 50x50.
- There will be more Components in future but it depends on the possibilities of the vaadin framework. A new default theme with statically bound add-ons to use in further components.

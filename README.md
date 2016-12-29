# MinecraftAnnotations
External fixes for `@Nullable`/`@Nonnull` annotations in the Minecraft source code, for mods that want strict and correct null annotations.  

These annotations are applied to decompiled MCP names, so they will need to be updated when the names change. Hopefully this project will remain small, there are not a huge number of wrong annotations in Minecraft.

## How to use these annotations in your project in IntelliJ Idea
 1. Fork and checkout this project to your computer using git.  
 (to `E:\code\MinecraftAnnotations` in this example)
 
 2. Enable External Annotations in IntelliJ
  * Go to `File -> Settings` (`Ctrl+Alt+S`).
  * On the left, navigate to `Editor -> Code Style -> Java`.
  * Select the `Code Generation` tab at the top right
  * Enable the `Use external annotations` checkbox at the very bottom.  
  (you may have to scroll down to see it)
  
 ![](http://i.imgur.com/2Ilv5GT.png)
  
 3. Add MinecraftAnnotations to your Project's Minecraft Source
  * In IntelliJ go to `File -> Project Structure` (`Ctrl+Alt+Shift+S`)
  * Select `Modules` on the left
  * Select your `main` module
  * Select `forgeSrc`, which is the decompiled Minecraft source code
   ![](http://i.imgur.com/gquHu0y.png)
  * Click the pencil icon on the right to edit it.
  * Use the plus icon at the left to add the `MinecraftAnnotations` folder.  
  It will automatically show up as Annotations, it should look like the image below.  
     ![](http://i.imgur.com/2CcV6CL.png)
  
## How to add your own annotations and contribute
  * Highlight a method, field, or parameter you want to annotate.
  * Type `Alt+Enter` to open the `Show Intention Actions` menu.
  * Choose the annotation you want  
   ![](http://i.imgur.com/IEhyls4.png)
  * If it asks you where you want to save external annotations, choose the MinecraftAnnotations directory.
  * Make a PR to this project with your fixes so that everyone can benefit!
  
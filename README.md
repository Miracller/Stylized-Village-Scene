# Stylized-Village-Scene

This is a repo to show my self-made stylized scene.

This is a preview image of the scene.
![image](https://raw.githubusercontent.com/Miracller/Stylized-Village-Scene/refs/heads/main/preview1.png)


Here is a video to demonstrate the scene.

https://github.com/user-attachments/assets/4363ae44-e18e-47dc-9d5d-69978d1514b4

---

## Technical Details

 1. Overall
    
    This scene mainly contains the following parts:
    - Terrain
    - Buildings
    - Foliages
    - Waters
      
    Our artists used **UE5** to edit the terrain and foliages parts, so I needed to use **UE5** to export assets into fbx format and then imported into Unity. In this stage, I also used **Blender** to adjust assets.

    Then I arranged every asset to its coherent position and added suitable components (like the Mesh Renderer or C# scripts) in Unity.

2. Shader part
   
     After that, I added shaders to each part of the scene. In details:
    - the tree leaves need a SSS shader, while tree barks need a tiling shader;
    - the waterfall needs vertex offset to reshape itself and rim light to emphysize the edges;
    - the lake shader needs mirror-like effect, water waves and foam effect;
    - the building needs a Metallic Roughness workflow PBR shader, etc.

4. Shadows & lightmap
   
    Next, I set the lights and cameras and adjusted the shadows (mainly cascade shadows). For artifacts, I had to change the ShadowCaster part in shaders.
   
    ![shadow1](https://github.com/user-attachments/assets/3a651040-b19e-4290-9718-33e2f35621a2)


    I used lightmap to bake large objects in the scene and light probes for smaller objects to keep bake times down.
   
    ![lightprobes](https://github.com/user-attachments/assets/98041260-8352-46f8-9fbe-eba570e8e503)

  
6. VFX & postprocessing

   I added some height fogs into the scene to make distant objects appear more hazy.

   I added falling leaves VFX.

   Fianlly, I added Color Grading, Blooming, AO, Exposure as postprocessing to the scene to enhance the visual experience.
   

    
    
    



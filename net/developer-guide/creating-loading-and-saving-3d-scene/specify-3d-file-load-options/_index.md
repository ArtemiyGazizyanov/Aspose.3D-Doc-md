---
title: Specify 3D File Load Options
type: docs
weight: 30
url: /net/specify-3d-file-load-options/
---

## **3D File Load Options**
There are several [Scene.Open](https://apireference.aspose.com/3d/net/aspose.threed/scene) method overloads or Scene class constructor overloads that accept a LoadOptions object. This should be an object of a class derived from the LoadOptions class. Each load format has a corresponding class that holds load options for that load format, for example there is ColladaSaveOptions for the FileFormat.Collada save format.
### **Use of the Discreet 3DS Load Options**
The code below shows how to set load options before loading a Discreet 3DS file.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-Discreet3DSOption.cs" >}}
### **Use of the Obj Load Options**
The code below shows how to set load options before loading an 3D Obj file.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-ObjLoadOption.cs" >}}
### **Use of the STL Load Options**
The code below shows how to set load options before loading an STL file.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-STLLoadOption.cs" >}}
### **Use of the U3D Load Options**
The code below shows how to set load options before loading a U3D file.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-U3DLoadOption.cs" >}}
### **Use of the glTF Load Options**
The code below shows how to set load options before loading a glTF file.
#### **Flip the V/T Texture Coordinate**
{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-glTFLoadOptions.cs" >}}
### **Use of the Ply Load Options**
The code below shows how to set load options before loading a PLY model.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-PlyLoadOptions.cs" >}}
### **Use of the DirectX X Load Options**
The code below shows how to set load options before loading a DirectX X file.

{{< gist "aspose-3d" "631532eeb21c3374f2ed" "Examples-CSharp-Loading-and-Saving-LoadOptions-XLoadOptions.cs" >}}
### **Use RVM load options**
**C#**

{{< highlight java >}}

 // set load options of RVM

Scene scene = new Scene();

var opt = new RvmLoadOptions()

{

    CylinderRadialSegments = 32,

    DishLatitudeSegments = 16,

    DishLongitudeSegments = 24,

    TorusTubularSegments = 40

};

// import RVM

scene.Open("LAD-TOP.rvm", opt);

// save in the OBJ format

scene.Save("LAD-TOP.obj", FileFormat.WavefrontOBJ);

{{< /highlight >}}
### **Using FBX Load Options**
{{< gist "aspose-com-gists" "15575b5bc038760ad09b3859ce2e3194" "Examples-CSharp-Loading-and-Saving-LoadOptions-FBXLoadOptions.cs" >}}

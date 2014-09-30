---
layout: page
title: Cutting planes demo (WPF)
---

Open the "ExampleBrowser" application to run this example.
The source code can be found in `Source\Examples\ExampleBrowser\Examples\CuttingPlanes`

This application demonstrates how to apply cutting planes to a model.
See [CONREC][conrec] for more information on the contour algorithm that is used to perform the cutting.

![Cutting planes demo](/public/images/demos/wpf/CuttingPlanesDemo.png)

``` xml
            <ht:CuttingPlaneGroup x:Name="cuttingGroup1">
                <ht:CuttingPlaneGroup.CuttingPlanes>
                    <ht:Plane3D Normal="0,-1,0"/>
                    <ht:Plane3D Normal="2,-1,0.1"/>
                </ht:CuttingPlaneGroup.CuttingPlanes>
                <ht:SphereVisual3D Center="0,0,2" BackMaterial="{ht:Material Blue}" Material="{ht:Material LightBlue}"/>
                <ht:CubeVisual3D Center="0.2,0.1,0" SideLength="2" BackMaterial="{ht:Material Green}" Material="{ht:Material LightGreen}"/>
                <ht:TruncatedConeVisual3D Origin="0.2,0.1,3" BackMaterial="{ht:Material Red}" Material="{ht:Material LightCoral}"/>
            </ht:CuttingPlaneGroup>
```

[conrec]: http://paulbourke.net/papers/conrec/
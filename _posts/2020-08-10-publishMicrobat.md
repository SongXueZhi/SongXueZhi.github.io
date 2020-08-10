---
typora-copy-images-to: upload
---

# Public  Microbat plug-In

This is a workflow for export the Eclipse plugin. Two method will be presented,1)export plugin project as a jar, and just copy the jar to Eclipse content plugins directory,2)export as a feature project which means you can install it in eclipse, moreover, update on website.

------



[TOC]

------

## Method1 

### Export as a plugin jars

#### Step 1, Select our Plugin project



<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp82ijoxj30k008qq3y.jpg" alt="image-20200810111838571" style="zoom:50%;" />

#### Step2, Export the  project as a  "Deployable plug-ins and fragments"



<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8bteamj30s00kudig.jpg" alt="image-20200810112053972" style="zoom:50%;" />

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp82xldcj30t60ugacm.jpg" alt="image-20200810112237391" style="zoom:50%;" />

#### Step3, Select all related jar, and finish

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8ae2i5j30x90u0gpm.jpg" alt="image-20200810112704009" style="zoom:50%;" />

#### Step4, Copy all jars to eclipse/plugins

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp83exm9j316o0o2djm.jpg" alt="image-20200810120646388" style="zoom:50%;" />

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp7th6yoj316o0o0wyo.jpg" alt="image-20200810120739062" style="zoom:50%;" />

#### At end, Restart  eclipse，Microbat will be effective.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8cctljj31av0u0111.jpg" alt="image-20200810121104141" style="zoom:50%;" />

### Remove the plugin

Just remove all jars that you copy to eclipse/plugins



## Method2

### Export as a feature project

#### Step 1, New a feature project.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp712iy0j30t20rqgpy.jpg" alt="image-20200810123239995" style="zoom:50%;" />



#### Step 2, Fill a project name

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp821ifsj30t00xudj1.jpg" alt="image-20200810134004552" style="zoom:50%;" />

#### Step 3, Next, and select our related jars

(microbat, mutation,sav.commons)

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp83ul9zj30sa0ucq5c.jpg" alt="image-20200810134227125" style="zoom:50%;" />

#### Step 4, Finish, and you can see more details in feature.xml

![image-20200810140610622](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp86tenij313u0u0dk7.jpg)

#### Step 5, New a Category Definition

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8d7ltqj30so0ritb4.jpg" alt="image-20200810134906578" style="zoom:50%;" />

Next, select all feature project and finish.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp80netdj30t60ugjuf.jpg" alt="image-20200810135113294" style="zoom:50%;" />

Then you can see a new file names "category.xml" under your project.

![image-20200810135145291](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp81frvbj30d603yweq.jpg)

Double click the file, and new a category.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp890tofj313p0u0tc9.jpg" alt="image-20200810135535094" style="zoom:50%;" />

Add feature, Select your feature project.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp84czjej30xi0ro0yx.jpg" alt="image-20200810135748834" style="zoom:50%;" />

#### Step 6,Export 

Export as a "Deployable features"

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8av47xj30yi0ty77e.jpg" alt="image-20200810135907910" style="zoom:50%;" />

Set your output directory

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp87msytj30xy0u00wr.jpg" alt="image-20200810140156554" style="zoom:50%;" />

Set Categorize repository in "Options " tag

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp815we7j30xm0u0dl0.jpg" alt="image-20200810140328560" style="zoom:50%;" />

Finish, and you can see the result in your output directory.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8680rpj316m0nyad8.jpg" alt="image-20200810140712250" style="zoom:50%;" />

Ok, now, you can install the feature in eclipse

### Update Site Project

#### Step 1, New a  Update Site Project

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp84wbjfj30sk0rs0vk.jpg" alt="image-20200810141534090" style="zoom:50%;" />

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp885qkhj30t40rsjtv.jpg" alt="image-20200810141556735" style="zoom:50%;" />

The project catalog

![image-20200810141738613](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8bc2wfj30de02aglq.jpg)

#### Step 2,Edit site.xml

New Category

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghloypbwngj312k0u0q78.jpg" alt="image-20200810141849060" style="zoom:50%;" />

Add Feature，and select the feature project

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp85lp1pj30ze0rygse.jpg" alt="image-20200810142022661" style="zoom:50%;" />

#### Step 3, build the project

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp8cotmgj30mq0s8abt.jpg" alt="image-20200810142200409" style="zoom:50%;" />

Then you can see the new structure in your site project.

<img src="https://tva1.sinaimg.cn/large/007S8ZIlgy1ghlp88kco6j30cs05kt91.jpg" alt="image-20200810142241552" style="zoom:50%;" />

#### Step 4, At end, you can copy the project catalog to your Apache server or the  others



 
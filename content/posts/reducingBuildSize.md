+++
title="Reducing Build Size"
date=2022-10-05
authors = ["Mark Rainey"]
[taxonomies]
categories=["coding"]
tags=[]

+++

I have been developing a Maui application as a side project and on the whole it has been a fun process. It is still very buggy and there are some pain points however it seems to work. One aspect I haven't liked is the size of the build artefacts - they are huge if you have multiple projects.

<!-- more -->

Patrick Smacchia posted an article which mentions a little known file called "Directory.Build.Props" which you can put in the root folder of your solution and it can, among other things, tell the build to use a single "bin" folder for the output. On my project this has saved over 1GB in output!

All you need to do is create the file in the same folder as the ".sln" file and include the following content:

```xml
<?xml version="1.0" encoding="utf-8"?>
<Project> 
   <PropertyGroup>
      <BaseOutputPath>..\bin</BaseOutputPath> 
   </PropertyGroup>
</Project>
```



__Links__

[.NET Build Improvement: Stop Wasting Resources](https://blog.ndepend.com/net-build-improvement-stop-wasting-resources/)


# About FreeCAD

<insert FreeCAD image>

FreeCAD [^1] is a free and open-source 3D modeling application. It runs on all major desktop operating systems such as Windows, Mac OS and GNU/Linux. Free and open-source software, or FLOSS, describes software which is free to use and redistribute without having to pay royalties or fees to the developers, and has its source code publicly available for anybody to use, study or modify.

FreeCAD has several features that makes it distinct from most other 3D modeling applications:

* FreeCAD is a **generic** 3D modeler. It is not tailored specifically for BIM or any other usage. This allows it to be useful for almost anybody in need for precise and very controllable 3D models, such as engineers, architects, product designers or for home 3D printing. Specific tools tailored for a particular usage, such as BIM, are also available, and grouped into workbenches. But you always have the whole range of other tools and workbenches at your disposal. There is nothing you can't model in FreeCAD.
* FreeCAD is a **parametric** modeler. Objects are defined by parameters, and their geometry is then generated automatically from these parameters. As an example, figure a brick that would be defined by length, width and height parameters. With these three dimensions, the program is able to create the rectangular shape of the brick. When we modify one of these dimensions, the program recalculates an updated shape. But parametric modeling goes way further than that in FreeCAD, and you can create complex chains of objects where you define what depends on what.
* FreeCAD is **feature-based**. Features are operations that you perform on a 3D object, such as adding or subtracting parts of it. Each feature is added on top of the previous state of the object. So your final object carries all its history of added or removed features, and it becomes very easy to navigate in that history and change one parameter if needed.
* FreeCAD is **NURBS and BREP based**. Although FreeCAD is also able to use other geometry types such as Mesh objects, its main geometry type is called *Boundary Representation*, or BRep [^2]. Boundary representation describes solid objects which are defined by a set of boundary surfaces. For example, a cube is defined by six boundary flat surfaces. These surfaces, in FreeCAD, are NURBS, or Non-Uniform Rational B-Spline [^3] surfaces. These surfaces are themselves defined by bordering B-Spline curves, which are mathematical functions that define for example lines, arcs or sinusoidal curves. To resume the whole thing, the position of any point on any object is actually the result of mathematical calculation. This makes objects highly precise and highly controllable, as the resulting surface can be modified by modifying the math behind each bordering curve. This is of course performed internally by the program, and transparent to the user, but always ensures a total precision, specifically on curves.
* FreeCAD is very deeply **customizable and extensible** using the *Python* [^4] programming language.  Python is very easy to learn, yet very powerful as it can make use of a huge collection of additional libraries. Almost half of FreeCAD itself is programmed in Python, and extending it can be as simple as copying and pasting a few lines of Python code to define a new tool, which we call a macro, or programming new, complete suites of tools, objects and user interfaces, which in FreeCAD we call a workbench.
* FreeCAD is developed by a **community** of volunteers. Most of us work on FreeCAD for the pleasure and interest of developing a 3D modeling application as we dream it, free of commercial constraints. Some write actual code, others take care of writing or translating the documentation and maintaining it updated, or  help new users to solve problems. Some developers are highly-skilled programmers, other are users who learned to code. This rich ecosystem is a fundamental piece of the success of FreeCAD, which is able to compete in several areas with commercial products.

## BIM functionality in FreeCAD

FreeCAD is at its base a generic application, not tailored specifically for one particular use. However, each group of users has, over the time, developed specific tools for their needs. These tools are grouped into what we call *workbenches*. The **BIM workbench** [^5] is where BIM tools are found, but there are other workbenches for example for ship design, or CNC machining.

In FreeCAD, you can switch at any moment between workbenches, and continue working on the same model. This allows you to take advantage of other tools not necessarily developed with BIM in mind, or permits designers from non-BIM areas to use any of the BIM tools. Workbenches are highly configurable,  and you can even design your own by picking your favorite tools from all over FreeCAD.

The BIM workbench in FreeCAD includes tools commonly found in other BIM applications, to build walls, beams, columns or windows, or produce automatic quantity tables or 2D drawings such as  plans or sections, but also brings in a lot of additional features coming from other parts of FreeCAD, such as the ability to draw and annotate directly on the 3D model. The BIM workbench also has a high level of compatibility with the IFC file format.

<talk about NativeIFC>

## Learning FreeCAD

This book will treat almost exclusively of BIM, but learning other areas and workbenches of FreeCAD will expand a lot what you can achieve with it. FreeCAD has an extensive user documentation [^6], with tutorials and a manual [^7] available in e-book forms.

---

[^1]: https://www.freecadweb.org
[^2]: https://en.wikipedia.org/wiki/Boundary_representation
[^3]: https://en.wikipedia.org/wiki/Non-uniform_rational_B-spline
[^4]: https://en.wikipedia.org/wiki/Python_(programming_language)
[^5]: https://www.freecadweb.org/wiki/BIM_Workbench
[^6]: https://www.freecadweb.org/wiki
[^7]: https://wiki.freecadweb.org/Manual

## RapCAD

#Introduction

RapCAD is an integrated development environment that allows for the creation of rapid prototype models using RepRap 3D printing machines. Unlike most CAD packages, RapCAD is not GUI based. One of the benefits of this is that it allows for designs to be described with a modular scene description language, providing compatibility with traditional text-based source control management software. This also allows for the creation of re-usable component modules that can be distributed as a design library.

Often the way traditional CAD packages are used is by creating temporary construction lines that are either deleted or put on an invisible layer. From a collaborator's perspective, it’s not always obvious how the final design was constructed. Using traditional source control management allows the transcript of decisions made during the design process to be recorded.

#Key Features and Benefits

- **Arbitrary precision arithmetic**: RapCAD uses arbitrary precision arithmetic, powered by the GMP and MPFR libraries, to perform calculations with very high precision. All calculations in the scene description script are made using precision arithmetic, and conversion to floating point precision is only done at the final output stage, which is either when the model is rendered and displayed using OpenGL, or the model is exported to file. This is important for certain types of modeling and design work, as it allows users to create more accurate models and handle complex geometric shapes.

- **Boolean operations on 3D Nef Polyhedrons**: RapCAD allows users to perform Boolean operations (such as union, intersection, and difference) on 3D Nef Polyhedrons, which are a type of geometric object used in computational geometry. This method is very robust, as it is capable of handling non-manifold objects, which are objects that have more than one surface at a single point. This is a useful feature for creating more complex models and manipulating shapes in precise ways.

- **Combined 2D/3D**: With RapCAD, there is no need to switch between separate 2D and 3D subsystems. Users can work with both 2D and 3D objects within the same environment, making it convenient to use RapCAD for a wide range of design tasks.

- **Multi-threaded operation for faster performance**: RapCAD is designed to take advantage of multi-core processors, which allows it to perform calculations more quickly. This can be especially useful for users who are working on large or complex models.

- **Support for procedural/imperative approach**: As a scene description language, RapCAD allows users to create and manipulate 3D models using a procedural/imperative programming approach. This means that users can write code to define the steps needed to create a 3D model, allowing them to automate tasks and create reusable components. The modular nature of the scene description language also makes it easier to work with large or complex models by breaking them down into smaller, more manageable pieces.

# annotation-processors: Part 1

An example on how to use Java Annotation Processors for with plain **javac**. To test the example, you will need an installed JDK 8.

Compile the Annotation Processor:

```
javac -cp . -proc:none com/cloudogu/blog/annotationprocessor/log/*.java
```

Compile the Hello class:

```
javac -cp . com/cloudogu/blog/annotationprocessor/sample/Hello.java
```

During the compilation of the Hello class, you should see an output from the Annotation Processor like the following:

```
Note: found @Log at com.cloudogu.blog.annotationprocessor.sample.Hello
```

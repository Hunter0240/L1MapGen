L1JMapGen
--------------------

- What does it do? -
This is a tool that processes maps described in V2Map format and makes them usable by an L1J (Lineage 1 Japan) server.

- What is output? -
Analysis results of V1Map and V2Map files
MAP_INFO information for TextMapReader
All tile information for the server

- How should I use it? -
1. Open ./config/config.properties and edit LineageMapDirectory to the correct path.
2. From the command line, navigate to the L1JMapGen directory.
3. Run: java -jar l1jmapgen.jar

- Warnings appear in Eclipse -
This is because the libraries required for testing are missing.
If you need to run tests, please add the following libraries to a 'lib' directory:
  asm-3.3.1.jar
  cglib-2.2.jar
  easymock-3.0.jar
  objenesis-1.2.jar
Since the source code of the tool itself does not reference these libraries, building is possible even without them.

- License -
Do as you like / Feel free

- Acknowledgements -
For the V1 map analysis, L1MapTool was used as a reference. Thank you very much.
I am using the modified version available on the author's website.
Download Link: https://assignmentchef.com/product/solved-cs1501-project-5-algorithms-to-perform-mathematical-operations-on-large-integers
<br>
To get hands on experience with algorithms to perform mathematical operations on large integers.

<h1>High-level description</h1>

You will be writing a replacement for Java’s BigInteger to perform multiplications and to run the extended Euclidean algorithm on integer values that would overflow long .

<h1>Specifications</h1>

<ol>

 <li>You are provided with the start of a class to process arbitrarily-sized integers called HeftyInteger . HeftyInteger objects are represented internally as <u><a href="https://en.wikipedia.org/wiki/Two%27s_complement">two’s-complement</a></u> <em>raw integers</em> using byte arrays (i.e., instances of byte[] ).</li>

 <li>Currently, HeftyInteger has the following operations implemented:</li>

</ol>

A constructor that creates a new HeftyInteger object based on a provided byte[] .

A method to compute the sum of two HeftyInteger objects.

A method to determine the negation of a HeftyInteger object.

A method to compute the difference of two HeftyInteger objects.

Several other helper methods.

<ol start="2">

 <li>Due to the use of a two’s complement representation of the integers, positive HeftyInteger objects should always have at least one leading 0 bit (indicating that the integer is positive) in their byte[] This property may cause the array to be bigger than expected (e.g., a 1024-bit positive integer will be represented using a length 129 byte array).</li>

 <li>HeftyIntegers are represented using a <em>big-endian</em> byte-order, so the most significant byte is at index 0 of the byte[] .</li>

 <li>You will further need to implement the following functions:</li>

</ol>

HeftyInteger multiply(HeftyInteger other)

HeftyInteger[] XGCD(HeftyInteger other)

Any additional helper functions that you deem necessary.

<ol start="5">

 <li>You may <em>not</em> use any calls the Java API class math.BigInteger or any other JCL class within HeftyInteger .</li>

 <li>Once HeftyInteger is complete, make sure your implementation of HeftyInteger can be used to run the driver programs contained in MultiplicationTest.java and XgcdTest.java . To get full credit, your implementation should be efficient enough to complete multiplication or XGCD given 200digit inputs within 3 minutes.</li>

</ol>
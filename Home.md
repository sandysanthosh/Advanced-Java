Welcome to the Advanced-Java wiki!



java fundamentals
packing
miscellanour enhance
assertions
regular expression
the java collection classes
generics
advanced io
enhanced io
logging api
networking
thread and concurrency
remote method invocation(RMI)
JDBC


naming conventions:

classname-Car
function name-getAge
varible names-age
contsant name-max length

reserved words
variable scope
primitive data types


string literal to obtain best performance
string s1="hello";

string s2=new string("hello");  //explicitly create a new object in memory

String Buffer:

StringBufferDemo st=new StringBufferDemo();
characters thatr can be modified
string manipulation 
string conacatenate

String str = new string("hello");
str += "stanford";

StringBuffer strb=new StringBuffer("Hello");
strb.append("stanfaord");

performance wise string buffer is faster

time difference between performance:


public void StringBufferDemo(){
sysout("long time");
long starttime=system.currentTimeMillis();
String concat=new StringBuffer(BUFFSIZE);
for(int i=0;i<iterations;i++)
{
concat.append(i%10);
}
long endTime=system.currentTimeMillis();
System.out.println("length"+concat.length());
System.out.println("length"+endTime - startTime);
}
}


public void String(){
sysout("long time");
long starttime=system.currentTimeMillis();
String concat=new String(BUFFSIZE);
for(int i=0;i<iterations;i++)
{
conact+=i%10;
}
long endTime=system.currentTimeMillis();
System.out.println("length"+concat.length());
System.out.println("length"+endTime - startTime);
}

void main(){
stringBufferDemo st=new stringBufferDemo ();
st.StringBufferDemo();
st.String();
}


Arrays:


->group of variables called elements

primitive type array:

int[] c=new int[2];

reference type array:

String[] b=new String[100];

int[] myarray;
myarray = new int[10];

int[] array={10,20,30,40};


sysout();

for(int i=0;i<array.length();i++)
{
sysout("%5d%8d\n",i,array[i]);
}

value of array:
{
sysout("%5d%8s\n","position","value");
}

For Each:

for(int number:array)
{
sop("%13d\n",number);
}

int [][] grid={
{3,5,2548},
{2,4},
{1,2,3,4},
};
s.o.p(grid[1][1]);
}
}


map:

hashmap
linkedhashmap
treemap

public static void testMap(Map<Interget,String> Map)
{
map.put(9,"fox");
for(Integer key:map.keySet()){
string value=map.get(key);
sysout();

}


set:

hashset--no order ,no duplicate
linkedhashset--insertion order, no duplicate
treeset---natural oerder ,no duplicate

methods:

contains
clear
clone
add
addAll
removeAll
retainAll
size
isEmpty
first
last


treeset:

custom objects in sets and as keys in map:


synchirnziantion in javaL


regex:

matches
find
group
start
end
group

pattern:

compile
macther
split
pattern

regex:
[abc]-simple abc
[^abc]-expect abc
[a-zA-Z]-inclusive
[a-d[m-p]]-union
[a-d&&[def]]-itersection
[a-d&&[^bc]]-subtraction
[a-d&[^m-p]]-a thorugh z


quantifiers:
x?-once or not at all
x+-one or more
x*-one or more
x{n}- ntimes

metachar:

\d-digit
\D-non digit
\s-whitepace
\S-non-white

time:

ZoneId
LocalTime
Year
Period
Duration
Instant

convert string to int:
int i=Integer.pasrseInt();
String.valueOf()
long l=Long.parseLong("200");

string to char:

char[] c=s1.toCharArray();

Strign to  date:

Date da=new SimpleDateFormat("dd-MM-yyyy").parse(s);

char to string:
String s=String.ValueOf(c);

String to object:

String s="hello";
Object obj=s;

object to string:

Emp e=new Emp();
String s=e.toString();
String s2=String.valueOf(e);

convert into long:

int i=200;
long l=i;

long to int:

long l= 500;
int i=(int)l;
double d=i;
int i=(int)d;
char c=(char)i;

execute java:

public class mylist
{
String[] list=null;

public mylist()
{
}
public 

mylist list=new mylist();
list.add("item1");
list.add("item2");
list.add("item3");

for(int i=0;i<list.size;i++)
{

}

exception:

suppose there are 10 exception found statement 5 will not execute.
witout statement 5 other code will execute in exception

checked:
->ioexception,sqlexception

unchecked:
->arithmetic exception,
null pointer exception,
ArrayIndexoutofBoundsException

jdbc:

register the driver
create connection
create stement
execute query
closig connections


jdom:

String:

<customer>
    <age>35</age>
    <name>aaa</name>
</customer>

SAXBuilder builder = new SAXBuilder();
File xmlFile = new File("c:\\file.xml");
Document document = (Document) builder.build(xmlFile);
Element rootNode = document.getRootElement();
List list = rootNode.getChildren("customer");

for (int i = 0; i < list.size(); i++) {

    Element node = (Element) list.get(i);

    System.out.println("Age : " + node.getChildText("age"));
    System.out.println("Name : " + node.getChildText("name"));         
}

jdom:
dwr.xml:
jaxb:
->convert object to xml  and xml to object

dwr:

java servlet running on the server that process requests and send response back to browser
javascript running in the browser sends request and can dynamically update the web page


patinetfax.js
dwr.xml
loadrh
Bo 
Dao

web.xml:
<servlet>
<servlet-name>dwr-invoker</servlet-name>
<servlet-class>org.directwebremoting.servlet.Dwrservlet</servlet-class>
<init-param>
<param-value>debug</param-value>
<param-value>true</param-value>
</init-param>
<init-param>
<param-value>crossDomainSession</param-value>
<param-value>false</param-value>
</init-param>
</servlet>


<mime-mapping>
<extension>pdf</extension>
<mime-type>application/pdf</mime-type>
</mime-mapping>

<filter>
<filet-name>timout</filter-name>
<display-name>timeout</display-name>
<filter-class>com.test.timoutFilter</filet-class>
</filter>


dwr.xml:

<dwr>
<allow>
<create creator="new" javascript="mscpatientdocs"/>
<param name="class" value="com.test.pojo.loadrh"/>
<include method="getinbound">
<include method="outobund">
<include method="getpending">
</create>
</allow>
</dwr>

https://www.geeksforgeeks.org/category/programming-language/java/
http://www.java2novice.com/java-interview-programs/



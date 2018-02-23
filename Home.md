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





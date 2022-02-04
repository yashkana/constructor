# constructor<br>
using System;<br>
namespace constructor<br>
{<br>
    class RegisterNum<br>
    {<br>
        int regno;<br>
    static int startnNum;<br>
        static RegisterNum()<br>
        {<br>
            startnNum = 20210000;<br>
        }<br>
        RegisterNum()<br>
        {<br>
            regno = ++startnNum;<br>
        }<br>
        static void Main(string[] args)<br>
        {<br>
            for(int i=0;i<100;i++)<br>
            {<br>
                RegisterNum student = new RegisterNum();<br>
                Console.WriteLine("student{0}:{1}", i + 1, student.regno);<br>
            }<br>    
        }<br>
    }<br>
}<br>

OUTPUT
![Screenshot 2022-02-04 065647](https://user-images.githubusercontent.com/98301023/152485833-c024a386-4989-4b78-8aa1-e376e00ce720.png)


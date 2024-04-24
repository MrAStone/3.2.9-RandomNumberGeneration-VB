<pre lang=vb.net>
Module Module1

    Sub Main()
        Dim r As New Random ' always at the start of the program
        Console.WriteLine(r.Next(1, 100)) ' numbers from 1 to 99 included in possible outcomes
        Dim a, b, c As Integer
        a = r.Next(1, 50)
        b = r.Next(50, 100)
        c = r.Next(991, 3201)
        Console.WriteLine($"{a} {b} {c}")
        Console.WriteLine(a + b + c)
        For i = 0 To 9
            Console.WriteLine(r.Next(1, 10))
        Next

    End Sub
    Function FunctionUsingRandom(n As Random, max As Integer)
        Return n.Next(1, max)
    End Function

End Module

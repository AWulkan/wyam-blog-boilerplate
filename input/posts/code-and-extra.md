Title: Code and Extra
Published: 4/10/2017
Tags: ExampleTag
---
Lorem ipsum dolor sit amet, `console.log('Look at me!');`. Sed maximus augue in ullamcorper vehicula. Fusce dui ipsum, ornare ut enim non, laoreet efficitur tortor. Suspendisse eget gravida sem. Aliquam eget lacinia eros. Orci varius natoque penatibus et magnis `console.log("I'm a string.");`, nascetur ridiculus mus.

**Checklist**
- [x] This is a complete item
- [ ] This is an incomplete item

**Four space indented code**

    if (isAwesome){
        return true;
    }

**Code fencing without styling**
```
if (isAwesome){
    return true;
}
```

**Code fencing with C# styling**
```cs
class DynamicPredicates : StudentClass
{
    static void Main(string[] args)
    {
        string[] ids = { "111", "114", "112" };

        Console.WriteLine("Press any key to exit.");
        Console.ReadKey();
    }

    static void QueryByID(string[] ids)
    {
        var queryNames =
            from student in students
            let i = student.ID.ToString()
            where ids.Contains(i)
            select new { student.LastName, student.ID };

        foreach (var name in queryNames)
        {
            Console.WriteLine($"{name.LastName}: {name.ID}");
        }
    }
}
```

**Code fencing with JS styling**
```js
var paramsString = "q=URLUtils.searchParams&topic=api"
var searchParams = new URLSearchParams(paramsString);

//Iterate the search parameters.
for (let p of searchParams) {
    console.log(p);
}

searchParams.has("topic") === true; // true
searchParams.get("topic") === "api"; // true
searchParams.getAll("topic"); // ["api"]
searchParams.get("foo") === null; // true
searchParams.append("topic", "webdev");
searchParams.toString(); // "q=URLUtils.searchParams&topic=api&topic=webdev"
searchParams.set("topic", "More webdev");
searchParams.toString(); // "q=URLUtils.searchParams&topic=More+webdev"
searchParams.delete("topic");
searchParams.toString(); // "q=URLUtils.searchParams"
```

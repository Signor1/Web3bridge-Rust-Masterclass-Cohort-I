## Summary of Chapter 5 & 6 of the Rust Book

### Structs

Imagine you have a bunch of information about a person: a name, an email address, and an age. Instead of keeping these as three separate, floating pieces of information, a struct lets you create a single "Person" blueprint. This blueprint says that every "Person" must have a name, an email, and an age.

So, a struct is just a way to bundle related information together and give it a single, meaningful name. It’s like creating a custom contact card template.

This chapter also explains that you can attach actions to your blueprints. If the "Person" blueprint is the noun, an action is a verb. For example, you could define an action called "check if adult" that belongs to the "Person" blueprint. This keeps your data and the things you can do with that data neatly organized together.

### Enums

First, we have enums (short for enumerations). An enum is a way to say that a value can only be one of a few specific things. Think of a traffic light: it can only be Red, Green, or Yellow. An enum lets you define a "TrafficLight" type that is limited to only those three possibilities.

The special thing about Rust's enums is that each possibility can hold different information. For example, you could create a "Transportation" enum. One option could be Car, which holds information about its make and model. Another option could be Bus, which holds its route number. This lets you express complex ideas very clearly.

This chapter also introduces the most important enum in Rust, called Option. It's used when a value might exist, or it might not. An Option is either Some (meaning, yes, the value is here) or None (meaning, no, there's nothing here). Rust forces you to handle the None case, which prevents a huge category of bugs common in other languages.

Second, we have pattern matching. This is the tool you use to handle enums. If you have a value that could be one of several possibilities (like our "Transportation" enum), a match statement lets you check which one it is and do something different for each case.

It’s like a super-smart switch. It looks at your value and says, "Okay, this is a Car, so I'll run the car code. Oh, this one is a Bus, so I'll run the bus code instead." The best part is that Rust forces you to have a plan for every single possibility, so you can't accidentally forget to handle a case. This makes your programs extremely reliable.

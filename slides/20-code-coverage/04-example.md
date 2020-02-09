### Code coverage example

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) {
  return customer.age >= 18;
}
```

```csharp
// Test
var customer = new Customer { name: 'Professor X', age: 96 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

What is the code coverage here?

😞 100% 😞 <!-- .element class="fragment" data-fragment-index="0" -->
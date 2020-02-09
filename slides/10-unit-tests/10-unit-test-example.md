## Unit test example

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) {
  return customer.age >= 18;
}
```

```csharp
// Test
var customer = new Customer { name: 'Mark', age: 24 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

An example of a unit test in c#
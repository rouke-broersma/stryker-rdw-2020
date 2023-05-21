## Mutating code

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) 
{
    return customer.age >= 18;
}   
```

```csharp
// Test
var customer = new Customer { name: 'Mark', age: 24 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

---

## Mutant is killed

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) 
{
    return customer.age < 18;
}
```

```csharp
// Test
var customer = new Customer { name: 'Mark', age: 24 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

---

## Mutant survives

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) 
{
    return customer.age > 18;
}
```

```csharp
// Test
var customer = new Customer { name: 'Mark', age: 24 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

---

## Mutant survives

```csharp
// Production code
bool IsAllowedToBuyAlcohol(Customer customer) 
{
    return true;
}
```

```csharp
// Test
var customer = new Customer { name: 'Mark', age: 24 };
Assert.True(IsAllowedToBuyAlcohol(customer));
```

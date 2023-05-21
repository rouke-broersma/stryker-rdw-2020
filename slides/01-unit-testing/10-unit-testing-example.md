## Unit testing example

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

<!-- .element class="flavor-csharp" -->

```javascript
// Production code
function isAllowedToBuyAlcohol(customer) 
{
  return customer.age >= 18;
}
```

```javascript
// Test
var customer = { name: 'Mark', age: 24 };
expect(isAllowedToBuyAlcohol(customer)).to.equal(true);
```

<!-- .element class="flavor-javascript" -->

An example of unit testing in <span class="flavor-csharp">c#</span><span class="flavor-javascript">Javascript</span>
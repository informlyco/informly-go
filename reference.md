# Reference
## Contacts
<details><summary><code>client.Contacts.ListContacts() -> *informlygo.ListContactsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informlygo.ListContactsRequest{}
client.Contacts.ListContacts(
        context.TODO(),
        request,
    )
}
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**page:** `*int` 
    
</dd>
</dl>

<dl>
<dd>

**pageSize:** `*int` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.CreateContact(request) -> *informlygo.CreateContactResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informlygo.CreateContact{}
client.Contacts.CreateContact(
        context.TODO(),
        request,
    )
}
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**email:** `*string` 
    
</dd>
</dl>

<dl>
<dd>

**phone:** `*string` 
    
</dd>
</dl>

<dl>
<dd>

**firstname:** `*string` 
    
</dd>
</dl>

<dl>
<dd>

**lastname:** `*string` 
    
</dd>
</dl>

<dl>
<dd>

**jobtitle:** `*string` 
    
</dd>
</dl>

<dl>
<dd>

**company:** `*string` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.GetContact(ID) -> *informlygo.GetContactResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informlygo.GetContactRequest{
        ID: "id",
    }
client.Contacts.GetContact(
        context.TODO(),
        request,
    )
}
```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**id:** `string` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>


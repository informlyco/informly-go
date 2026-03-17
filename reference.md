# Reference
## Contacts
<details><summary><code>client.Contacts.ListContacts() -> *informly.ListContactsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.ListContactsRequest{
        Page: informly.Int(
            1,
        ),
        PageSize: informly.Int(
            20,
        ),
    }
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

**page:** `*int` — Page number (1-indexed)
    
</dd>
</dl>

<dl>
<dd>

**pageSize:** `*int` — Number of items per page (1-100)
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.CreateContact(request) -> *informly.CreateContactResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.CreateContact{}
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

**email:** `*string` — Email address of the contact
    
</dd>
</dl>

<dl>
<dd>

**phone:** `*string` — Phone number of the contact
    
</dd>
</dl>

<dl>
<dd>

**firstname:** `*string` — First name of the contact
    
</dd>
</dl>

<dl>
<dd>

**lastname:** `*string` — Last name of the contact
    
</dd>
</dl>

<dl>
<dd>

**jobtitle:** `*string` — Job title of the contact
    
</dd>
</dl>

<dl>
<dd>

**company:** `*string` — Company of contact (if different) or organization name
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.GetContact(ID) -> *informly.GetContactResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.GetContactRequest{
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

**id:** `string` — Unique identifier of the resource
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>


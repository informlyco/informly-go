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

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Creates a new contact or updates an existing one if a contact with the same email or phone already exists. Optionally assigns segments and redeems a referral code.
</dd>
</dl>
</dd>
</dl>

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

**email:** `*string` — Email address. Required if phone is not provided.
    
</dd>
</dl>

<dl>
<dd>

**phone:** `*string` — Phone number in E.164 format. Required if email is not provided.
    
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

**company:** `*string` — Company or organization name
    
</dd>
</dl>

<dl>
<dd>

**segmentIDs:** `[]string` — Segment IDs to assign to the contact
    
</dd>
</dl>

<dl>
<dd>

**referralCode:** `*string` — Referral code to redeem for this contact
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.DeleteContacts(request) -> *informly.DeleteContactsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.DeleteContacts{
        IDs: []string{
            "ids",
        },
    }
client.Contacts.DeleteContacts(
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

**ids:** `[]string` — Contact IDs to delete
    
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

<details><summary><code>client.Contacts.UpdateContact(ID, request) -> *informly.UpdateContactResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Updates an existing contact's fields. If segmentIds is provided, it replaces all existing segment assignments.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.UpdateContact{
        ID: "id",
    }
client.Contacts.UpdateContact(
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

<dl>
<dd>

**email:** `*string` — Email address of the contact
    
</dd>
</dl>

<dl>
<dd>

**phone:** `*string` — Phone number in E.164 format (e.g. +14155552671)
    
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

**company:** `*string` — Company or organization name
    
</dd>
</dl>

<dl>
<dd>

**segmentIDs:** `[]string` — Segment IDs to assign (replaces existing segments)
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.Contacts.DeleteContact(ID) -> *informly.DeleteContactResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
request := &informly.DeleteContactRequest{
        ID: "id",
    }
client.Contacts.DeleteContact(
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

## Segments
<details><summary><code>client.Segments.ListSegments() -> *informly.ListSegmentsResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Returns all segments available in the organization.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```go
client.Segments.ListSegments(
        context.TODO(),
    )
}
```
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>


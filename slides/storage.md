build-lists: true
footer: IDM 231: Scripting for IDM I
slidenumbers: true
autoscale: true
theme: Cobalt2, 1

# IDM 231

## Scripting for Interactive Digital Media I

### Client-side Storage

---

# Objectives

- Introduce Client-side Storage Techniques
- Discuss Web Storage
- Discuss IndexedDB

---

# Objective

## Introduce Client-side Storage Techniques

---

> Web Storage

^ Modern browsers offer web storage that can be processed by JavaScript on the browser. Web storage can be used to store approximately 5mb of data. When you use web storage, you can use either _local storage_ or _session storage_. The difference is that items in local storage persist between browser sessions, but items in session storage are removed when the browser session ends.

---

## Local vs Session Storage

- `setItem`
- `getItem`
- `removeItem`
- `clear`

^ To work with local and session storage, which store items in name/value pairs, you use the `setItem`, `getItem`, `removeItem` and `clear` methods.

---

```javascript
01 localStorage.setItem('email', 'grace@gmail.com');
02 const email = localStorage.getItem('email');
03
04 localStorage.email = 'grace@gmail.com';
05 const email = localStorage.email;
```

---

```javascript
01 sessionStorage.setItem('itemname', 'value');
02 const itemName = sessionStorage.getItem('itemname');
03
04 sessionStorage.removeItem('itemname');
05 sessionStorage.clear();
```

^ _Show storage tab in devTools_

---

# Objective

## Discuss IndexedDB

---

## IndexedDB

- [IndexedDB Documentation](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Client-side_web_APIs/Client-side_storage#Storing_complex_data_—_IndexedDB)

^ The IndexedDB API (sometimes abbreviated IDB) is a complete database system available in the browser in which you can store complex related data, the types of which aren't limited to simple values like strings or numbers. You can store videos, images, and pretty much anything else in an IndexedDB instance.

^ However, this does come at a cost: IndexedDB is much more complex to use than the Web Storage API. We're not going to dive deep into this concept now, but it is a topic you should learn more about once you're comfortable with the Web Storage techniques.

---
description: >-
  이 장의 지침이 일관성 있게 적용되면 코드상의 identifiers(type, members, parameters) 들을 쉽게 파악 할수
  있습니다.
---

# 대문자 표기법

## identifiers에 대한 대문자 규칙

identifiers 에서 단어 구별을 위해 각 단어의 첫 문자를 대문자로 표기 하십시오. identifiers 에서 단어를 구별하기 위해 밑줄을 사용하지 마십시오. 사용 용도에 대문자로 표시하는 두 가지 방법이 있습니다.

* [ ] PascalCasing  :  \[ **E**xample**N**ame \] &lt;-- all public member, type, namespace
* [ ] camelCasing   :  \[ **e**xample**N**ame \] &lt;-- parameter

PascalCasing 은 parameter 를 제외한 모든 identifiers 에 사용되며, 각 단어의 첫 문자를 대문자로 표시합니다. 다음과 같이 사용됩니다.

 `PropertyDescriptor` `HtmlTag`

약어의 경우는 하나의 단어로 취급하며 모두 대문자로 표시합니다. 다음과 같이 사용됩니다.

`IOStream`

camelCasing 은 parameter 만을 위해 사용되며, 첫 단어를 제외한 단어의 첫 문자를 대문자로 표시합니다. 다음과 같이 사용되며, 약어의 경우는 camelCasing 에 따라 모두 소문자로 표시합니다.

`propertyDescriptor` `htmlTag`  `ioStream`



다음 표는 다양한 유형의 identifiers 에 대한 대문자 규칙을 설명합니다.

| Identifier | Casing | Example |
| :---: | :--- | :--- |
| Namespace | Pascal | `namespace System.Security { ... }` |
| Type | Pascal | `public class StreamReader { ... }` |
| Interface | Pascal | `public interface IEnumerable { ... }` |
| Method | Pascal | `public class Object {`     `public virtual string ToString();` `}` |
| Property | Pascal | `public class String {`     `public int Length { get; }` `}` |
| Event | Pascal | `public class Process {`     `public event EventHandler Exited;` `}` |
| Field | Pascal | `public class MessageQueue {`     `public static readonly TimeSpan`     `InfiniteTimeout;` `}` `public struct UInt32 {`     `public const Min = 0;` `}` |
| Enum value | Pascal | `public enum FileMode {`     `Append,`    `...` `}` |
| Parameter | Camel | `public class Convert {`     `public static int ToInt32(string value);` `}` |

## 복합 단어에 대한 대문자 표기  

대문자 표기법의 목적을 위하여 복합 단어는 하나의 단어로 취급 합니다. 즉, `endpoint` 와 같은 복합 단어를 하나의 단어로를 취급합니다. 아래 표를 사용하여 하나의 단어로 취급할 복합 단어를 확인 합니다.

| Pascal | Camel | Not |
| :--- | :--- | :--- |
| `BitFlag` | `bitFlag` | `Bitflag` |
| `Callback` | `callback` | `CallBack` |
| `Canceled` | `canceled` | `Cancelled` |
| `DoNot` | `doNot` | `Don't` |
| `Email` | `email` | `EMail` |
| `Endpoint` | `endpoint` | `EndPoint` |
| `FileName` | `fileName` | `Filename` |
| `Gridline` | `gridline` | `GridLine` |
| `Hashtable` | `hashtable` | `HashTable` |
| `Id` | `id` | `ID` |
| `Indexes` | `indexes` | `Indices` |
| `LogOff` | `logOff` | `LogOut` |
| `LogOn` | `logOn` | `LogIn` |
| `Metadata` | `metadata` | `MetaData, metaData` |
| `Multipanel` | `multipanel` | `MultiPanel` |
| `Multiview` | `multiview` | `MultiView` |
| `Namespace` | `namespace` | `NameSpace` |
| `Ok` | `ok` | `OK` |
| `Pi` | `pi` | `PI` |
| `Placeholder` | `placeholder` | `PlaceHolder` |
| `SignIn` | `signIn` | `SignOn` |
| `SignOut` | `signOut` | `SignOff` |
| `UserName` | `userName` | `Username` |
| `WhiteSpace` | `whiteSpace` | `Whitespace` |
| `Writable` | `writable` | `Writeable` |




---
description: '이 섹션에서는 일반적인 이름을 사용할때 단어 선택, 약어 사용 및 언어 별 예약어 사용을 피하는 방법에 대하여 설명 합니다.'
---

# 일반 이름 표기

## 단어 선택

{% hint style="success" %}
쉽게 읽을 수 있는 이름을 선택 합니다.

AligmentHorizontal 보다 **HorizontalAligment** 가 이름에 적합합니다.
{% endhint %}

{% hint style="success" %}
간결함보다 가독성에 중점을 둡니다.

X축에 대한 동작으로 ScrollableX 보다 **CanScrollHorizontally** 가 이름에 적합합니다.
{% endhint %}

{% hint style="danger" %}
underscores\(\_\) , hyphens\(-\) 혹은 알파벳이 아닌 다른 글자를 사용하지 않습니다.
{% endhint %}

{% hint style="danger" %}
헝가리안 표기법을 사용하지 않습니다.
{% endhint %}

{% hint style="danger" %}
널리 사용되는 프로그래밍 언어의 키워드와 충돌하는 식별자는 사용하지 않습니다.

Common Language Specification\(CLS\)의 규칙 4 에 따르면,  모든 호환 언어는 해당 언어의 키워드를 식별자로 사용하는 명명된 항목에 액세스 할 수 있는 메커니즘을 제공 해야 합니다. 예를 들어 C\#의 경우 @ 기호를 이스케이프 메커니즘으로 사용합니다. 그러나 이스케이프 시퀀스가 없는 메소드보다 이스케이프 시퀀스가 있는 메소드를 사용하는 것이 훨씬 어렵기 때문에 일반적인 키워드를 사용하지 않는 것이 좋습니다.
{% endhint %}

## 약어나 줄임말 사용

{% hint style="danger" %}
식별자의 이름으로 약어나 줄임말을 사용하지 않습니다.

예를들어, GetWin 보다 **GetWindow** 를 사용 합니다.
{% endhint %}

{% hint style="danger" %}
널리 인정되지 않는 줄임말은 사용하지 않습니다.
{% endhint %}

{% hint style="success" %}
필요한 경우에만 줄임말을 사용합니다.
{% endhint %}

## 예약어 사용을 피하는 방법

{% hint style="success" %}
이름에 언어별 예약어 대신 의미적으로 파악하기 쉬운 이름을 사용하십시오.

예를들어, GetInt 보다 **GetLength** 가 이름으로 더 좋습니다.
{% endhint %}

{% hint style="success" %}
드문 경우이지만 이름에 형식 이상의 의미가 없는 경우에는 언어별 이름 대신 일반 CLR 형식 이름을 사용하십시오.

예를 들어 Int64로 변환하는 메서드의 이름은 ToLong이 아니라 **ToInt64**로 지정 해야합니다. \(Int64는 CLR 형식 이름이며 C\# 에서는 long으로 표현됩니다\).
{% endhint %}

다음 표는 CLR 형식 이름 \(C \#, Visual Basic 및 C ++에 대한 해당 형식 이름\)을 사용하는 몇 가지 기본 데이터 형식을 보여줍니다.

| C\# | Visual Basic | C++ | CLR |
| :--- | :--- | :--- | :--- |
| **sbyte** | **SByte** | **char** | **SByte** |
| **byte** | **Byte** | **unsigned char** | **Byte** |
| **short** | **Short** | **short** | **Int16** |
| **ushort** | **UInt16** | **unsigned short** | **UInt16** |
| **int** | **Integer** | **int** | **Int32** |
| **uint** | **UInt32** | **unsigned int** | **UInt32** |
| **long** | **Long** | **\_\_int64** | **Int64** |
| **ulong** | **UInt64** | **unsigned \_\_int64** | **UInt64** |
| **float** | **Single** | **float** | **Single** |
| **double** | **Double** | **double** | **Double** |
| **bool** | **Boolean** | **bool** | **Boolean** |
| **char** | **Char** | **wchar\_t** | **Char** |
| **string** | **String** | **String** | **String** |
| **object** | **Object** | **Object** | **Object** |

{% hint style="success" %}
의미와 변수의 유형이 중요하지 않은 경우, 이름을 반복하지 않고 값이나 항목과 같은 공통 이름을 사용하십시오.
{% endhint %}

## 존재하는 API의 새로운 이름

{% hint style="success" %}
기존 API의 새 버전을 작성할 때 이전 API와 유사한 이름을 사용하십시오.

이를 통해 API 간의 관계를 강조 할 수 있습니다.
{% endhint %}

{% hint style="success" %}
기존 API의 새 버전을 나타 내기 위해 접두사 대신 접미사를 추가하는 것을 선호합니다.

이것은 문서를 탐색하거나 IntelliSense를 사용할 때 관련 검색을 지원합니다. 대부분의 브라우저와 IntelliSense는 식별자를 알파벳 순서로 표시하므로 이전 버전의 API는 새로운 API에 가깝게 구성됩니다.
{% endhint %}

{% hint style="info" %}
접미사 또는 접두사를 추가하는 대신 새롭지만 의미있는 이름의 사용을 고려합니다.
{% endhint %}

{% hint style="success" %}
숫자 접미사를 사용하여 기존 API의 새 버전을 나타냅니다. 특히 API의 기존 이름이 의미가 있는 유일한 이름\(즉, 산업표준인 경우\)이고 의미있는 접미사를 추가하는 것\(또는 이름 변경\)이 적절한 옵션이 아닌 경우에 해당합니다.
{% endhint %}

{% hint style="danger" %}
동일한 API의 이전 버전과 구별하기 위해 식별자에 "Ex"\(또는 유사한\) 접미사를 사용하지 마십시오.
{% endhint %}

{% hint style="success" %}
32 비트 정수 대신 64 비트 정수 \(long integer\)에서 작동하는 API 버전을 도입 할 때는 "64"접미사를 사용하십시오. 기존 32 비트 API가 존재하는 경우에만이 방법을 사용해야합니다. 64 비트 버전의 새로운 API에는 사용하지 마십시오.
{% endhint %}


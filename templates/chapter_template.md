# Chapter X: [챕터 제목]

## 📖 학습 목표
이 챕터를 완료하면 다음을 할 수 있습니다:
- [목표 1]
- [목표 2]
- [목표 3]

## 📋 목차
1. [섹션 1]
2. [섹션 2]
3. [섹션 3]
4. 실습 예제
5. 확인 문제

---

## 1. [섹션 1 제목]

### 개념 설명
[이론적 내용 설명]

### 시각적 자료
```mermaid
[적절한 다이어그램]
```

> **💡 팁**
> <div style="background-color: #daa520; padding: 10px; border-radius: 5px;">
> [유용한 팁이나 주의사항]
> </div>

---

## 2. [섹션 2 제목]

### [하위 주제 1]
[상세 설명]

### [하위 주제 2]
[상세 설명]

> **⚠️ 주의사항**
> <div style="background-color: #c35b5b; padding: 10px; border-radius: 5px;">
> [중요한 주의사항이나 경고]
> </div>

---

## 3. [섹션 3 제목]

### [하위 주제]
[설명]

> **✅ 성공 포인트**
> <div style="background-color: #3cb371; padding: 10px; border-radius: 5px;">
> [성공적인 구현을 위한 포인트]
> </div>

---

## 🔧 실습 예제

### 예제 1: [예제 제목]

**목표**: [예제의 학습 목표]

**전제 조건**:
- Java 8 이상
- Maven 또는 Gradle
- IDE (IntelliJ IDEA 권장)

#### Java 코드 예제

```java
// 패키지 선언 - 프로젝트의 구조를 나타냄
package com.example.ignite;

// 필요한 라이브러리 임포트
import org.apache.ignite.Ignite;        // Ignite 메인 인터페이스
import org.apache.ignite.Ignition;      // Ignite 인스턴스 생성을 위한 클래스
import org.apache.ignite.IgniteCache;   // 캐시 작업을 위한 인터페이스

/**
 * [클래스 설명]
 * - 이 클래스는 [목적] 위해 작성되었습니다
 * - [주요 기능 설명]
 */
public class ExampleClass {
    
    public static void main(String[] args) {
        // Ignite 인스턴스 시작 - 기본 설정으로 노드를 시작합니다
        Ignite ignite = Ignition.start();
        
        try {
            // [코드 설명 - 각 라인별로 상세한 설명]
            
        } finally {
            // 리소스 정리 - 항상 Ignite 인스턴스를 종료해야 합니다
            ignite.close();
        }
    }
}
```

#### 프로젝트 구조
```
src/
└── main/
    └── java/
        └── com/
            └── example/
                └── ignite/
                    └── ExampleClass.java
```

**파일 위치 설명**:
- `src/main/java`: Java 소스 코드의 표준 Maven 디렉토리
- `com.example.ignite`: 패키지명 (회사/프로젝트명.기술명 패턴)
- 이는 MVC 패턴에서 Model 계층에 해당

#### Maven 의존성 (pom.xml)
```xml
<dependency>
    <groupId>org.apache.ignite</groupId>
    <artifactId>ignite-core</artifactId>
    <version>2.16.0</version>
</dependency>
```

### 예제 2: JavaScript/React 연동 (해당하는 경우)

```javascript
// React 컴포넌트에서 Ignite REST API 활용
import React, { useState, useEffect } from 'react';

const IgniteComponent = () => {
    // 상태 관리 - React의 useState 훅 사용
    const [data, setData] = useState(null);
    const [loading, setLoading] = useState(false);
    
    // Ignite REST API 호출 함수
    const fetchDataFromIgnite = async () => {
        setLoading(true);
        try {
            // REST API를 통한 데이터 조회
            const response = await fetch('http://localhost:8080/ignite?cmd=get&key=myKey');
            const result = await response.json();
            setData(result);
        } catch (error) {
            console.error('Error fetching data:', error);
        } finally {
            setLoading(false);
        }
    };
    
    return (
        <div>
            {/* 컴포넌트 렌더링 로직 */}
        </div>
    );
};

export default IgniteComponent;
```

---

## ✅ 확인 문제

### 문제 1 (단일 선택)
[문제 내용]

1. [선택지 1]
2. [선택지 2]
3. [선택지 3]
4. [선택지 4]

### 문제 2 (복수 선택)
[문제 내용] (해당하는 것을 모두 선택하세요)

1. [선택지 1]
2. [선택지 2]
3. [선택지 3]
4. [선택지 4]

### 문제 3 (실습 문제)
[실제 코드를 작성하거나 수정하는 문제]

---

## 📚 정리

### 핵심 내용 요약
- [요점 1]
- [요점 2]
- [요점 3]

### 다음 챕터 준비
다음 챕터에서는 [다음 내용 예고]에 대해 학습합니다.

---

## 🔗 참고 자료
- [Apache Ignite 관련 공식 문서 링크]
- [추가 학습 자료]

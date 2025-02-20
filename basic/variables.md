# 변수형

## 목차
- [var](#var)
- [dynamic](#dynamic)
- [Object](#object)
- [String?](#string)
- [late](#late)
- [final](#final)
- [const](#const)

## var
var type1 = "String";<br>
var type2 = 123;<br>
type1은 String형, type2는 int형이됨<br><br>
**특징:**
 - 어떤걸 넣어도 상관없음
 - 한번 정해진 타입은 안바뀜

## dynamic
dynamic type1 = "String";<br>
dynamic type2 = 123;<br>
 - String a = type1; 가능
 - String a = type2; 오류<br>
type1, type2는 dynamic형<br><br>
**특징:**
 - 어떤걸 넣어도 상관없음
 - 저장되는 값에 형태가 같으면 Stringdp에 dynamic형도 저장가

## Object
Object type1 = "String";<br>
Object type2 = 123;<br>
 - String a = type1 as String; 가능
 - String a = type1 is String; 가능
 - String a = type1; 오류<br>
type1, type2는 dynamic형<br><br>
**특징:**
 - dart최상위 타입
 - 어떤걸 넣어도 상관없음
 - 다른 타입에 값을 저장하려면 as나 is를 사용해야함 -> 타입 안정성 보장

## String?
String? a;<br>
 - 값이 null일수 있을때 ?를 붙임

## late
late String a;<br>
a = 'acb';<br><br>
**특징:**
 - 초기화를 선언과 같이 안해도됨
 - 변수 초기화에 this에 대한 접근이 필요하면 사용

## final
final a1 = 'String';<br>
final String a2 = 'String';<br><br>
**특징:**
 - 한번만 값을 지정가능(실행중에 값을 지정가능)
 - 타입을 지정하든 안하든 상관없음

## const
const a = 'String';<br><br>
**특징:**
 - 빌드시에만 값이 정해지고 안바뀜(실행중에 값을 입력 불가능)
 - 타입을 지정하든 안하든 상관없음

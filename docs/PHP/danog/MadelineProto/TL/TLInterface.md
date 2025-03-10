---
title: "danog\\MadelineProto\\TL\\TLInterface: "
description: ""
image: "https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png"
parent: "MadelineProto API"

---
# `danog\MadelineProto\TL\TLInterface`
[Back to index](../../../index.html)

> Author: Daniil Gentili <daniil@daniil.it>  
  

  




## Method list:
* [`getConstructors(): \danog\MadelineProto\TL\TLConstructors`](#getconstructors-danog-madelineproto-tl-tlconstructors)
* [`getMethods(): \danog\MadelineProto\TL\TLMethods`](#getmethods-danog-madelineproto-tl-tlmethods)
* [`getDescriptions(): array`](#getdescriptions-array)
* [`getMethodNamespaces(): array`](#getmethodnamespaces-array)
* [`getMethodsNamespaced(): array`](#getmethodsnamespaced-array)
* [`serializeObject(array $type, mixed $object, string $ctx, int $layer = -1): mixed`](#serializeobject-array-type-mixed-object-string-ctx-int-layer-1-mixed)
* [`serializeMethod(string $method, mixed $arguments): mixed`](#serializemethod-string-method-mixed-arguments-mixed)
* [`getLength(\resource|string $stream, array $type = [  'type' => '',]): int`](#getlength-resource-string-stream-array-type-type-int)
* [`getSideEffects(): ?\Amp\Future`](#getsideeffects-amp-future)
* [`deserialize(string|\resource $stream, array $type): mixed`](#deserialize-string-resource-stream-array-type-mixed)

## Methods:
### `getConstructors(): \danog\MadelineProto\TL\TLConstructors`

Get constructors.


#### See also: 
* `\danog\MadelineProto\TL\TLConstructors`




### `getMethods(): \danog\MadelineProto\TL\TLMethods`

Get methods.


#### See also: 
* `\danog\MadelineProto\TL\TLMethods`




### `getDescriptions(): array`

Get descriptions.



### `getMethodNamespaces(): array`

Get TL namespaces.



### `getMethodsNamespaced(): array`

Get namespaced methods (method => namespace).



### `serializeObject(array $type, mixed $object, string $ctx, int $layer = -1): mixed`

Serialize TL object.


Parameters:

* `$type`: `array` TL type definition  
* `$object`: `mixed` Object to serialize  
* `$ctx`: `string` Context  
* `$layer`: `int` Layer version  



### `serializeMethod(string $method, mixed $arguments): mixed`

Serialize method.


Parameters:

* `$method`: `string` Method name  
* `$arguments`: `mixed` Arguments  



### `getLength(\resource|string $stream, array $type = [  'type' => '',]): int`

Get length of TL payload.


Parameters:

* `$stream`: `\resource|string` Stream  
* `$type`: `array` Type identifier  


#### See also: 
* `\resource`




### `getSideEffects(): ?\Amp\Future`




#### See also: 
* `\Amp\Future`




### `deserialize(string|\resource $stream, array $type): mixed`

Deserialize TL object.


Parameters:

* `$stream`: `string|\resource` Stream  
* `$type`: `array` Type identifier  


#### See also: 
* `\resource`




---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)

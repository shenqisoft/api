[Polkadot JS API](../README.md) › [Globals](../globals.md) › ["extrinsic/Extrinsic"](../modules/_extrinsic_extrinsic_.md) › [Extrinsic](_extrinsic_extrinsic_.extrinsic.md)

# Class: Extrinsic

**`name`** GenericExtrinsic

**`description`** 
Representation of an Extrinsic in the system. It contains the actual call,
(optional) signature and encodes with an actual length prefix

[https://github.com/paritytech/wiki/blob/master/Extrinsic.md#the-extrinsic-format-for-node](https://github.com/paritytech/wiki/blob/master/Extrinsic.md#the-extrinsic-format-for-node).

Can be:
- signed, to create a transaction
- left as is, to create an inherent

## Hierarchy

* ExtrinsicBase

  ↳ **Extrinsic**

## Implements

* [Codec](../interfaces/_types_codec_.codec.md)
* [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)

## Index

### Constructors

* [constructor](_extrinsic_extrinsic_.extrinsic.md#constructor)

### Properties

* [registry](_extrinsic_extrinsic_.extrinsic.md#registry)

### Accessors

* [args](_extrinsic_extrinsic_.extrinsic.md#args)
* [argsDef](_extrinsic_extrinsic_.extrinsic.md#argsdef)
* [callIndex](_extrinsic_extrinsic_.extrinsic.md#callindex)
* [data](_extrinsic_extrinsic_.extrinsic.md#data)
* [encodedLength](_extrinsic_extrinsic_.extrinsic.md#encodedlength)
* [era](_extrinsic_extrinsic_.extrinsic.md#era)
* [hasOrigin](_extrinsic_extrinsic_.extrinsic.md#hasorigin)
* [hash](_extrinsic_extrinsic_.extrinsic.md#hash)
* [isEmpty](_extrinsic_extrinsic_.extrinsic.md#isempty)
* [isSigned](_extrinsic_extrinsic_.extrinsic.md#issigned)
* [length](_extrinsic_extrinsic_.extrinsic.md#length)
* [meta](_extrinsic_extrinsic_.extrinsic.md#meta)
* [method](_extrinsic_extrinsic_.extrinsic.md#method)
* [nonce](_extrinsic_extrinsic_.extrinsic.md#nonce)
* [signature](_extrinsic_extrinsic_.extrinsic.md#signature)
* [signer](_extrinsic_extrinsic_.extrinsic.md#signer)
* [tip](_extrinsic_extrinsic_.extrinsic.md#tip)
* [type](_extrinsic_extrinsic_.extrinsic.md#type)
* [version](_extrinsic_extrinsic_.extrinsic.md#version)

### Methods

* [addSignature](_extrinsic_extrinsic_.extrinsic.md#addsignature)
* [eq](_extrinsic_extrinsic_.extrinsic.md#eq)
* [sign](_extrinsic_extrinsic_.extrinsic.md#sign)
* [signFake](_extrinsic_extrinsic_.extrinsic.md#signfake)
* [toHex](_extrinsic_extrinsic_.extrinsic.md#tohex)
* [toHuman](_extrinsic_extrinsic_.extrinsic.md#tohuman)
* [toJSON](_extrinsic_extrinsic_.extrinsic.md#tojson)
* [toRawType](_extrinsic_extrinsic_.extrinsic.md#torawtype)
* [toString](_extrinsic_extrinsic_.extrinsic.md#tostring)
* [toU8a](_extrinsic_extrinsic_.extrinsic.md#tou8a)

## Constructors

###  constructor

\+ **new Extrinsic**(`registry`: [Registry](../interfaces/_types_registry_.registry.md), `value`: [Extrinsic](_extrinsic_extrinsic_.extrinsic.md) | ExtrinsicValue | [AnyU8a](../modules/_types_helpers_.md#anyu8a) | Call | undefined, `__namedParameters`: object): *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:174](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L174)*

**Parameters:**

▪ **registry**: *[Registry](../interfaces/_types_registry_.registry.md)*

▪ **value**: *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md) | ExtrinsicValue | [AnyU8a](../modules/_types_helpers_.md#anyu8a) | Call | undefined*

▪`Default value`  **__namedParameters**: *object*= {}

Name | Type |
------ | ------ |
`version` | undefined &#124; number |

**Returns:** *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

## Properties

###  registry

• **registry**: *[Registry](../interfaces/_types_registry_.registry.md)*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md).[registry](../interfaces/_types_extrinsic_.iextrinsic.md#registry)*

*Inherited from [Base](_codec_base_.base.md).[registry](_codec_base_.base.md#registry)*

*Defined in [packages/types/src/codec/Base.ts:17](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/codec/Base.ts#L17)*

## Accessors

###  args

• **get args**(): *[Codec](../interfaces/_types_codec_.codec.md)[]*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[args](_extrinsic_extrinsic_.extrinsic.md#args)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:45](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L45)*

**`description`** The arguments passed to for the call, exposes args so it is compatible with [Call](_generic_call_.call.md)

**Returns:** *[Codec](../interfaces/_types_codec_.codec.md)[]*

___

###  argsDef

• **get argsDef**(): *[ArgsDef](../modules/_types_codec_.md#argsdef)*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[argsDef](_extrinsic_extrinsic_.extrinsic.md#argsdef)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:52](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L52)*

**`description`** The argument definitions, compatible with [Call](_generic_call_.call.md)

**Returns:** *[ArgsDef](../modules/_types_codec_.md#argsdef)*

___

###  callIndex

• **get callIndex**(): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[callIndex](_extrinsic_extrinsic_.extrinsic.md#callindex)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:59](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L59)*

**`description`** The actual `[sectionIndex, methodIndex]` as used in the Call

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

___

###  data

• **get data**(): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[data](_extrinsic_extrinsic_.extrinsic.md#data)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:66](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L66)*

**`description`** The actual data for the Call

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

___

###  encodedLength

• **get encodedLength**(): *number*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[encodedLength](_extrinsic_extrinsic_.extrinsic.md#encodedlength)*

*Overrides [Base](_codec_base_.base.md).[encodedLength](_codec_base_.base.md#encodedlength)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:80](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L80)*

**`description`** The length of the value when encoded as a Uint8Array

**Returns:** *number*

___

###  era

• **get era**(): *[ExtrinsicEra](_extrinsic_extrinsicera_.extrinsicera.md)*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[era](_extrinsic_extrinsic_.extrinsic.md#era)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:73](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L73)*

**`description`** The era for this extrinsic

**Returns:** *[ExtrinsicEra](_extrinsic_extrinsicera_.extrinsicera.md)*

___

###  hasOrigin

• **get hasOrigin**(): *boolean*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[hasOrigin](_extrinsic_extrinsic_.extrinsic.md#hasorigin)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:87](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L87)*

**`description`** `true` is method has `Origin` argument (compatibility with [Call])

**Returns:** *boolean*

___

###  hash

• **get hash**(): *H256*

*Inherited from [Base](_codec_base_.base.md).[hash](_codec_base_.base.md#hash)*

*Defined in [packages/types/src/codec/Base.ts:36](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/codec/Base.ts#L36)*

**`description`** returns a hash of the contents

**Returns:** *H256*

___

###  isEmpty

• **get isEmpty**(): *boolean*

*Inherited from [Base](_codec_base_.base.md).[isEmpty](_codec_base_.base.md#isempty)*

*Defined in [packages/types/src/codec/Base.ts:43](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/codec/Base.ts#L43)*

**`description`** Checks if the value is an empty value

**Returns:** *boolean*

___

###  isSigned

• **get isSigned**(): *boolean*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[isSigned](_extrinsic_extrinsic_.extrinsic.md#issigned)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:94](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L94)*

**`description`** `true` id the extrinsic is signed

**Returns:** *boolean*

___

###  length

• **get length**(): *number*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[length](_extrinsic_extrinsic_.extrinsic.md#length)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:101](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L101)*

**`description`** The length of the actual data, excluding prefix

**Returns:** *number*

___

###  meta

• **get meta**(): *FunctionMetadataLatest*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[meta](_extrinsic_extrinsic_.extrinsic.md#meta)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:108](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L108)*

**`description`** The [[FunctionMetadataLatest]] that describes the extrinsic

**Returns:** *FunctionMetadataLatest*

___

###  method

• **get method**(): *Call*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[method](_extrinsic_extrinsic_.extrinsic.md#method)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:115](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L115)*

**`description`** The [Call](_generic_call_.call.md) this extrinsic wraps

**Returns:** *Call*

___

###  nonce

• **get nonce**(): *[Compact](_codec_compact_.compact.md)‹Index›*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[nonce](_extrinsic_extrinsic_.extrinsic.md#nonce)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:122](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L122)*

**`description`** The nonce for this extrinsic

**Returns:** *[Compact](_codec_compact_.compact.md)‹Index›*

___

###  signature

• **get signature**(): *EcdsaSignature | Ed25519Signature | Sr25519Signature*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[signature](_extrinsic_extrinsic_.extrinsic.md#signature)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:129](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L129)*

**`description`** The actual [[EcdsaSignature]], [[Ed25519Signature]] or [[Sr25519Signature]]

**Returns:** *EcdsaSignature | Ed25519Signature | Sr25519Signature*

___

###  signer

• **get signer**(): *Address*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[signer](_extrinsic_extrinsic_.extrinsic.md#signer)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:136](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L136)*

**`description`** The [Address](_generic_address_.address.md) that signed

**Returns:** *Address*

___

###  tip

• **get tip**(): *[Compact](_codec_compact_.compact.md)‹Balance›*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[tip](_extrinsic_extrinsic_.extrinsic.md#tip)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:143](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L143)*

**`description`** Forwards compat

**Returns:** *[Compact](_codec_compact_.compact.md)‹Balance›*

___

###  type

• **get type**(): *number*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[type](_extrinsic_extrinsic_.extrinsic.md#type)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:150](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L150)*

**`description`** Returns the raw transaction version (not flagged with signing information)

**Returns:** *number*

___

###  version

• **get version**(): *number*

*Inherited from [Extrinsic](_extrinsic_extrinsic_.extrinsic.md).[version](_extrinsic_extrinsic_.extrinsic.md#version)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:157](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L157)*

**`description`** Returns the encoded version flag

**Returns:** *number*

## Methods

###  addSignature

▸ **addSignature**(`signer`: Address | [Uint8Array](_codec_raw_.raw.md#static-uint8array) | string, `signature`: [Uint8Array](_codec_raw_.raw.md#static-uint8array) | string, `payload`: [ExtrinsicPayloadValue](../interfaces/_types_extrinsic_.extrinsicpayloadvalue.md) | [Uint8Array](_codec_raw_.raw.md#static-uint8array) | string): *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:223](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L223)*

**`description`** Injects an already-generated signature into the extrinsic

**Parameters:**

Name | Type |
------ | ------ |
`signer` | Address &#124; [Uint8Array](_codec_raw_.raw.md#static-uint8array) &#124; string |
`signature` | [Uint8Array](_codec_raw_.raw.md#static-uint8array) &#124; string |
`payload` | [ExtrinsicPayloadValue](../interfaces/_types_extrinsic_.extrinsicpayloadvalue.md) &#124; [Uint8Array](_codec_raw_.raw.md#static-uint8array) &#124; string |

**Returns:** *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

___

###  eq

▸ **eq**(`other?`: any): *boolean*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Inherited from [Base](_codec_base_.base.md).[eq](_codec_base_.base.md#eq)*

*Defined in [packages/types/src/codec/Base.ts:50](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/codec/Base.ts#L50)*

**`description`** Compares the value of the input to see if there is a match

**Parameters:**

Name | Type |
------ | ------ |
`other?` | any |

**Returns:** *boolean*

___

###  sign

▸ **sign**(`account`: [IKeyringPair](../interfaces/_types_interfaces_.ikeyringpair.md), `options`: [SignatureOptions](../interfaces/_types_extrinsic_.signatureoptions.md)): *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:232](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L232)*

**`description`** Sign the extrinsic with a specific keypair

**Parameters:**

Name | Type |
------ | ------ |
`account` | [IKeyringPair](../interfaces/_types_interfaces_.ikeyringpair.md) |
`options` | [SignatureOptions](../interfaces/_types_extrinsic_.signatureoptions.md) |

**Returns:** *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

___

###  signFake

▸ **signFake**(`signer`: Address | [Uint8Array](_codec_raw_.raw.md#static-uint8array) | string, `options`: [SignatureOptions](../interfaces/_types_extrinsic_.signatureoptions.md)): *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:241](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L241)*

**`describe`** Adds a fake signature to the extrinsic

**Parameters:**

Name | Type |
------ | ------ |
`signer` | Address &#124; [Uint8Array](_codec_raw_.raw.md#static-uint8array) &#124; string |
`options` | [SignatureOptions](../interfaces/_types_extrinsic_.signatureoptions.md) |

**Returns:** *[Extrinsic](_extrinsic_extrinsic_.extrinsic.md)*

___

###  toHex

▸ **toHex**(`isBare?`: undefined | false | true): *string*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Overrides [Base](_codec_base_.base.md).[toHex](_codec_base_.base.md#tohex)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:250](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L250)*

**`description`** Returns a hex string representation of the value

**Parameters:**

Name | Type |
------ | ------ |
`isBare?` | undefined &#124; false &#124; true |

**Returns:** *string*

___

###  toHuman

▸ **toHuman**(`isExpanded?`: undefined | false | true): *[AnyJson](../modules/_types_helpers_.md#anyjson)*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Overrides [Base](_codec_base_.base.md).[toHuman](_codec_base_.base.md#tohuman)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:257](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L257)*

**`description`** Converts the Object to to a human-friendly JSON, with additional fields, expansion and formatting of information

**Parameters:**

Name | Type |
------ | ------ |
`isExpanded?` | undefined &#124; false &#124; true |

**Returns:** *[AnyJson](../modules/_types_helpers_.md#anyjson)*

___

###  toJSON

▸ **toJSON**(): *string*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Overrides [Base](_codec_base_.base.md).[toJSON](_codec_base_.base.md#tojson)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:277](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L277)*

**`description`** Converts the Object to JSON, typically used for RPC transfers

**Returns:** *string*

___

###  toRawType

▸ **toRawType**(): *string*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Overrides [Base](_codec_base_.base.md).[toRawType](_codec_base_.base.md#torawtype)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:284](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L284)*

**`description`** Returns the base runtime type name for this instance

**Returns:** *string*

___

###  toString

▸ **toString**(): *string*

*Implementation of [IExtrinsic](../interfaces/_types_extrinsic_.iextrinsic.md)*

*Inherited from [Base](_codec_base_.base.md).[toString](_codec_base_.base.md#tostring)*

*Defined in [packages/types/src/codec/Base.ts:78](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/codec/Base.ts#L78)*

**`description`** Returns the string representation of the value

**Returns:** *string*

___

###  toU8a

▸ **toU8a**(`isBare?`: undefined | false | true): *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*

*Overrides [Base](_codec_base_.base.md).[toU8a](_codec_base_.base.md#tou8a)*

*Defined in [packages/types/src/extrinsic/Extrinsic.ts:292](https://github.com/polkadot-js/api/blob/d9dad3566a/packages/types/src/extrinsic/Extrinsic.ts#L292)*

**`description`** Encodes the value as a Uint8Array as per the SCALE specifications

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`isBare?` | undefined &#124; false &#124; true | true when the value is not length-prefixed  |

**Returns:** *[Uint8Array](_codec_raw_.raw.md#static-uint8array)*
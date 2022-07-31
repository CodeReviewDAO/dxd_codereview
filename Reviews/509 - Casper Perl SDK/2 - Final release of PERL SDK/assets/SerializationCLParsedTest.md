'''
1..76
ok 1 - Test serialization for CLParsed Bool true value passed
ok 2 - Test serialization for CLParsed Bool false value passed
ok 3 - Test serialization for CLParsed U8(0) value passed
ok 4 - Test serialization for CLParsed U8(9) value passed
ok 5 - Test serialization for CLParsed U8(219) value passed
ok 6 - Test serialization for CLParsed U8(255) value passed
ok 7 - Test serialization for CLParsed I32(0) value passed
ok 8 - Test serialization for CLParsed I32(-1024) value passed
ok 9 - Test serialization for CLParsed I32(-3333) value passed
ok 10 - Test serialization for CLParsed I32(1000) value passed
ok 11 - Test serialization for CLParsed I32(5005) value passed
ok 12 - Test serialization for CLParsed I32(12764) value passed
ok 13 - Test serialization for CLParsed I32(-12369) value passed
Serialize I64 for 0
ok 14 - Test serialization for CLParsed I64(0) value passed
I64 for minus number-1024
ok 15 - Test serialization for CLParsed I64(-1024) value passed
Serialize I64 for 1000
ok 16 - Test serialization for CLParsed I64(1000) value passed
I64 for minus number-123456789
ok 17 - Test serialization for CLParsed I64(-123456789) value passed
I64 for minus number-56789
ok 18 - Test serialization for CLParsed I64(-56789) value passed
Serialize I64 for 56789
ok 19 - Test serialization for CLParsed I64(56789) value passed
ok 20 - Test serialization for CLParsed U32(1024) value passed
ok 21 - Test serialization for CLParsed U32(5531024) value passed
ok 22 - Test serialization for CLParsed U32(0) value passed
ok 23 - Test serialization for CLParsed U32(334455) value passed
ok 24 - Test serialization for CLParsed U32(03100000) value passed
ok 25 - Test serialization for CLParsed U64(1024) value passed
ok 26 - Test serialization for CLParsed U64(33009900995531024) value passed
ok 27 - Test serialization for CLParsed U64(0) value passed
ok 28 - Test serialization for CLParsed U64(300000) value passed
ok 29 - Test serialization for CLParsed U64(123456789) value passed
ok 30 - Test serialization for CLParsed U128(123456789101112131415) value passed
ok 31 - Test serialization for CLParsed U128(1024) value passed
ok 32 - Test serialization for CLParsed U128(0) value passed
ok 33 - Test serialization for CLParsed U256(999988887777666655556666777888999) value passed
ok 34 - Test serialization for CLParsed U256(2048) value passed
ok 35 - Test serialization for CLParsed U256(0) value passed
ok 36 - Test serialization for CLParsed U512(999888666555444999887988887777666655556666777888999666999) value passed
ok 37 - Test serialization for CLParsed U512(4096) value passed
ok 38 - Test serialization for CLParsed U512(100000000) value passed
ok 39 - Test serialization for CLParsed U512(0) value passed
ok 40 - Test serialization for CLParsed String(Hello, World!) value passed
ok 41 - Test serialization for CLParsed String(lWJWKdZUEudSakJzw1tn) value passed
ok 42 - Test serialization for CLParsed String(S1cXRT3E1jyFlWBAIVQ8) value passed
ok 43 - Test serialization for CLParsed String(123456789123456789123456789123456789123456789123456789) value passed
ok 44 - Test serialization for CLParsed String(target) value passed
ok 45 - Test serialization for CLParsed String(Weather) value passed
ok 46 - Test serialization for CLParsed String(aa) value passed
ok 47 - Test serialization for CLParsed String(I want to know, really!) value passed
ok 48 - Test serialization for CLParsed Unit value passed
ok 49 - Test serialization for CLParsed Key(Account Hash) value passed
ok 50 - Test serialization for CLParsed Key(Hash) value passed
ok 51 - Test serialization for CLParsed Key(URef) value passed
ok 52 - Test negative serialization for CLParsed Key(abcdef) value passed
ok 53 - Test serialization for CLParsed URef value passed
ok 54 - Test serialization for CLParsed URef value passed
ok 55 - Test negative serialization for CLParsed URef value passed
ok 56 - Test serialization for CLParsed PublicKey value passed
ok 57 - Test serialization for CLParsed PublicKey value passed
ok 58 - Test serialization for CLParsed Option(NULL) value passed
ok 59 - Test serialization for CLParsed Option(U32(10)) value passed
ok 60 - Test serialization for CLParsed Option(U64(123456)) value passed
ok 61 - Test serialization for CLParsed Option(String(Hello, World!)) value passed
ok 62 - Test serialization for CLParsed List(empty) value passed
ok 63 - Test serialization for CLParsed List(U32) value passed
ok 64 - Test serialization for CLParsed List(String) value passed
ok 65 - Test serialization for CLParsed List(U8) value passed
ok 66 - Test serialization for CLParsed Map(String,String) value passed
ok 67 - Test serialization for CLParsed Map(String,String) 2 value passed
ok 68 - Test serialization for CLParsed ByteArray value passed
ok 69 - Test serialization for CLParsed Any value passed
ok 70 - Test serialization for CLParsed Result(Ok(String)) value passed
ok 71 - Test serialization for CLParsed Result(Err(U512)) value passed
ok 72 - Test serialization for CLParsed Result(Err(String)) value passed
ok 73 - Test serialization for CLParsed Tuple1(I32) value passed
ok 74 - Test serialization for CLParsed Tuple1(String) value passed
ok 75 - Test serialization for CLParsed Tuple2(String,U512) value passed
ok 76 - Test serialization for CLParsed Tuple3(PublicKey,Option(String),U512) value passed
'''
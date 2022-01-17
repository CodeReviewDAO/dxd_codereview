```
> Task :clean

> Task :generateMainEffectiveLombokConfig1

> Task :compileJava

> Task :processResources NO-SOURCE
> Task :classes
> Task :jar
> Task :assemble

> Task :generateTestEffectiveLombokConfig1

> Task :compileTestJava
> Task :processTestResources
> Task :testClasses

> Task :test

AccountInfoTests > validateAccountInfoMapping() PASSED

AuctionInfoTest > validateAuctionInfoMapping() PASSED

JsonBlockDataTest > validateJsonBlock_EraEndBlock() PASSED

CLValueTests > getTypeByName_from_CLTypeData_should_throw_NoSuchTypeException() PASSED

CLValueTests > createCLValueFromCLTypeName_from_CLTypeData_should_throw_NoSuchTypeException() PASSED

CLValueTests > getTypeBySerializationTag_should_return_correct_CLTypeData() PASSED

CLValueTests > createCLTypeFromCLTypeData_should_return_correct_CLType() PASSED

CLValueTests > getClassByName_from_CLTypeData_should_throw_NoSuchTypeException() PASSED

CLValueTests > getCLTypeClassByName_from_CLTypeData_should_throw_NoSuchTypeException() PASSED

CLValueTests > createCLValueFromCLTypeName_should_return_correct_CLValue() PASSED

CLValueTests > allCLTypes_must_be_implemented() PASSED

EncoderDecoderTests > dataWithWrongInputLength_should_throw_CLValueDecodeException() PASSED

EncoderDecoderTests > numbersShouldBeInsideTheirTypeBounds() PASSED

EncoderDecoderTests > dataOutOfBounds_should_throw_CLValueEncodeException() PASSED

EncoderDecoderTests > validateEncode_with_SampleData() PASSED

EncoderDecoderTests > validateDecode_with_SampleData() PASSED

DeployDataTests > validateDeployDataMapping_1() PASSED

DeployDataTests > validateDeployDataMapping_2() PASSED

DeployDataTests > validateDeployDataMapping_3() PASSED

DeployDataTests > validateDeployResultMapping() PASSED

DictionaryDataTest > validateDictionaryMapping() PASSED

StateRootHashTest > validateStateRootHashMapping() PASSED

StatusDataTests > validateStatusMapping() PASSED

StoredValueTests > validate_CLValueOption_Mapping_with_bool() PASSED

StoredValueTests > validate_CLValueMap_Mapping_with_string_tuple1_i32() PASSED

StoredValueTests > validate_Transfer_Mapping() PASSED

StoredValueTests > validate_CLValueTuple3_Mapping_with_i32_string_bool() PASSED

StoredValueTests > validate_CLValueTuple3_Mapping_with_tuple2_tuple1_u512_u512_tuple1_string_tuple1_bool() PASSED

StoredValueTests > validate_CLValueU256_Mapping() PASSED

StoredValueTests > validate_CLValueOption_Mapping_with_empty() PASSED

StoredValueTests > validate_CLValueList_Mapping_with_i32() PASSED

StoredValueTests > validate_CLValueResult_Mapping_with_i32_string() PASSED

StoredValueTests > validate_CLValueTuple1_Mapping_with_bool() PASSED

StoredValueTests > validate_CLValueFixedList_Mapping_with_tuple1_i32() PASSED

StoredValueTests > validate_CLValueURef_Mapping() PASSED

StoredValueTests > validate_CLValueMap_Mapping_with_string_i32() PASSED

StoredValueTests > validate_Contract_Mapping_with_access_as_groups() PASSED

StoredValueTests > validate_Contract_Mapping() PASSED

StoredValueTests > validate_CLValueList_Mapping_with_tuple2_i32_i32() PASSED

StoredValueTests > validate_CLValueString_Mapping() PASSED

StoredValueTests > validate_CLValuePublicKey_Mapping() PASSED

StoredValueTests > validate_CLValueTuple3_Mapping_with_tuple1_u512_string_bool() PASSED

StoredValueTests > validate_CLValueFixedList_Mapping_with_i32() PASSED

StoredValueTests > validate_CLValueAny_Mapping() PASSED

StoredValueTests > validate_CLValueKey_Mapping_of_hash() PASSED

StoredValueTests > validate_CLValueUnit_Mapping() PASSED

StoredValueTests > validate_CLValueTuple3_Mapping_with_u8_string_bool() PASSED

StoredValueTests > validate_CLValueResult_Mapping_with_i32_tuple1_string() PASSED

StoredValueTests > validate_CLValueFixedList_Mapping_with_i32_odd_byte_length() PASSED

StoredValueTests > validate_CLValueFixedList_Mapping_with_i32_wrong_byte_length() PASSED

StoredValueTests > validate_Account_Mapping() PASSED

StoredValueTests > validate_CLValueOption_Mapping_with_i32() PASSED

StoredValueTests > validate_CLValueOption_Mapping_with_tuple2_i32_string() PASSED

StoredValueTests > validate_CLValueU32_Mapping() PASSED

StoredValueTests > validate_CLValueByteArray_Mapping() PASSED

StoredValueTests > validate_CLValueU64_Mapping() PASSED

StoredValueTests > validate_CLValueKey_Mapping_of_account() PASSED

StoredValueTests > validate_CLValueI64_Mapping() PASSED

StoredValueTests > validate_CLValueTuple3_Mapping_with_tuple1_bool_string_bool() PASSED

StoredValueTests > validate_CLValueU8_Mapping() PASSED

StoredValueTests > validate_CLValueU128_Mapping() PASSED

StoredValueTests > validate_CLValueTuple2_Mapping_with_i32_string() PASSED

TransferDataTest > validateDictionaryMapping() PASSED

CasperServiceTests > getStateRootHashByHeight() PASSED

CasperServiceTests > getBlockByHeight() PASSED

CasperServiceTests > retrieveLastBlockStateRootHash() PASSED

CasperServiceTests > getAccountStateInfoByBlockHash() PASSED

CasperServiceTests > getStateItem_account() PASSED

CasperServiceTests > testIfBlockReturnedMatchesRequestedByHash() PASSED

CasperServiceTests > retrieveLastBlockTransfers() PASSED

CasperServiceTests > getEraInfoBySwitchBlockByHash() PASSED

CasperServiceTests > testFirstBlocksPublicKeySerialization() PASSED

CasperServiceTests > getBlockByHash() PASSED

CasperServiceTests > getAuctionInfoByBlockHash() PASSED

CasperServiceTests > getEraInfoBySwitchBlockByHeight() PASSED

CasperServiceTests > retrieveLastBlock() PASSED

CasperServiceTests > getDeploy() PASSED

CasperServiceTests > getStateRootHashByHash() PASSED

CasperServiceTests > getStatus() PASSED

CasperServiceTests > getTransferByHash() PASSED

CasperServiceTests > getBlockState() PASSED

CasperServiceTests > getAuctionInfoByBlockHeight() PASSED

CasperServiceTests > retrieveNonEmptyListOfPeers() PASSED

CasperServiceTests > getStateItem_contract() PASSED

CasperServiceTests > testIfBlockReturnedMatchesRequestedByHeight() PASSED

CasperServiceTests > getAccountStateInfoByBlockHeight() PASSED

CasperServiceTests > getTransferByHeight() PASSED

-----------------------------------------------------------------
|  Results: SUCCESS (87 tests, 87 passed, 0 failed, 0 skipped)  |
-----------------------------------------------------------------

> Task :jacocoTestReport
> Task :check
> Task :build

BUILD SUCCESSFUL in 17s
9 actionable tasks: 9 executed
```

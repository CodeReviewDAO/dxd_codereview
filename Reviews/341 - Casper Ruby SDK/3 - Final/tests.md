```bash
abahmane@Ubuntu-2004-focal-64-minimal:~/reviews/341-3/casper-ruby-sdk$ bundle exec rspec -fd

Utils::ByteUtils
  .string_to_hex
    convert string to hex
  .hex_to_string
    convert hex to string
  .hex_to_byte_array
    convert hex to byte_array
  .byte_array_to_hex
    convert byte_array to hex
  .byte_array_to_string
    convert byte_array to string
  .integer_to_hex
    convert integer to hex value
  .hex_to_integer
    convert hex to integer value
  .hex_from_little_endian_to_big_endian
    convert  hex little endian to hex big endian format

CLBool
  toBytes() / fromBytes() do proper bytes serialization
  #get_cl_type
    Bool should return proper cl_type
  #get_value
    should return proper value by calling get_value

CLString
  should return 'ABC'
  should do to_bytes / from_bytes string serialization
  #get_value
    should return proper value
  #get_cl_type
    should return proper cl_type
  #get_cl_type
    should return String type
  #cl_string.get_size
    should return proper string length

CLi32
  should do proper to_bytes and from_bytes when value is -1
  should do proper to_bytes and from_bytes when value is 0
  should do proper to_bytes and from_bytes when value is 1
  should do proper to_bytes and from_bytes when value is MIN_I32
  should do proper to_bytes and from_bytes when value is MAX_I32

CLi64
  should do proper to_bytes and from_bytes when value is -10
  should do proper to_bytes and from_bytes when value is 0
  should do proper to_bytes and from_bytes when value is 10
  should do proper to_bytes and from_bytes when value is MIN_I64
  should do proper to_bytes and from_bytes when value is MAX_I64

CLu8
  should do proper to_bytes and from_bytes when value is MIN_U8
  should do proper to_bytes and from_bytes when value is MAX_U8
  should raise error. Parameter value '-1' is not in range [0, 255]

CLu32
  should do proper to_bytes and from_bytes when value is MIN_U32
  should do proper to_bytes and from_bytes when value is MAX_U32
  should raise error. Parameter value  '-1' is out of range [0, MAX_U32]
  should raise error. Parameter value '4294967296' is out of range [0, MAX_U32]

CLu64
  should do proper to_bytes and from_bytes when value is MIN_U64
  should do proper to_bytes and from_bytes when value is MAX_U64
  should raise error. Parameter value  '-1' is out of range [0, MAX_U64]
  should raise error. Parameter value '18446744073709551616' is out of range [0, MAX_U64]

CLu128
  should do proper to_bytes and from_bytes when value is MIN_U128
  should do proper to_bytes and from_bytes when value is MAX_U128
  should raise error. Parameter value  '-1' is out of range [0, MAX_U128]
  should raise error. Parameter value '340282366920938463463374607431768211456' is out of range [0, MAX_U128]

CLu256
  should do proper to_bytes and from_bytes when value is MIN_U256
  should do proper to_bytes and from_bytes when value is MAX_U256
  should raise error. Parameter value  '-1' is out of range [0, MAX_U256]
  should raise error. Parameter value '115792089237316195423570985008687907853269984665640564039457584007913129639936' is out of range [0, MAX_U256]

CLu512
  should do proper to_bytes and from_bytes when value is MIN_U512
  should do proper to_bytes and from_bytes when value is MAX_U512
  should raise error. Parameter value  '-1' is out of range [0, MAX_U512]
  should raise error. Parameter value '13407807929942597099574024998205846127479365820592393377723561443721764030073546976801874298166903427690031858186486050853753882811946569946433649006084096' is out of range [0, MAX_U512]

CLUnit
  should return proper type
  should return proper value
  to_json / from_json

CLTuple
  CLTuple1
    should return proper CLType
    should throw an error when tuple elements are not in a correct format
    should return error when tuple is not correctly built
    should do proper to_bytes and from_bytes for Tuple1
  CLTuple2
    should return proper CLType
    should throw an error when tuple elements are not in a correct format
    should return error when tuple is not correctly built
    should do proper to_bytes and from_bytes for Tuple2
  CLTuple3
    should return proper CLType
    should throw an error when tuple elements are not in a correct format
    should return error when tuple is not correctly built

CLURef
  should return proper CLType
  should return proper value
  should return proper AccessRights
  should do proper to_bytes and from_bytes
  should return error when CLUref is not correctly built
  #parse_uref_address
    should raise an error when string does not begin with 'uref-'
    should raise an error when string does not begin with prefix: 'uref-'
    should raise an error when uref bytes length is not equal to 32
    should raise an error when given parameter has lack of suffix which represents AccessRights
    should raise an error when AccessRights is not within a range [0, 7]
    should convert to_json and from_json properly

CLPublicKey
  should return error when CLPublicKey is not correctly built
  should raise error when CLPublicKey is not properly constructed
  should return proper CLType
  to_hex / from_hex work properly for ed25519
  to_hex / from_hex work properly for secp256K1
  to_account_hash_byte_array works properly
  to_account_hash_hex works properly
  should do proper to_bytes and from_bytes serialization for CLPublicKey
  to_json / from_json for CLPublicKey

CLValueSerializer
  CLBool Value Serializer
    should serialize CLBool values
  CLi32 Value Serializer
    should serialize CLi32 values
  CLi64 Value Serializer
    should serialize CLi64 values
  CLu8 Value Serializer
    should serialize CLu8 values
  CLu32 Value Serializer
    should serialize CLu32 values
  CLu64 Value Serializer
    should serialize CLu64 values
  CLu512 Value Serializer
    should serialize CLu512 values
  CLString Value Serializer
    should serialize CLString values
  CLURef Value Serializer
    should serialize CLURef values
  CLPublicKey Value Serializer
    should serialize CLPublicKey values
  CLTuple
    CLTuple1
      should serialize CLTuple1
    CLTuple2
      should serialize CLTuple2
    CLTuple3
      should serialize CLTuple3
  CLUnit Value Serializer
    should serialize CLUnit values

Casper::RpcClient
  #info_get_peers
    returns peers array.
  #chain_get_StateRootHash
    returns current state_root_hash.

DeployApprovalSerializer
  should serialize DeployAproval

Casper::Entity::DeployExecutable
  Casper::Entity::ModuleBytes
    ModuleBytes serialization
  Casper::Entity::StoredContractByHash
    StoredContractByHash serialization
  Casper::Entity::StoredContractByName
    StoredContractByName serialization
  Casper::Entity::StoredVersionedContractByHash
    StoredVersionedContractByHash serialization
  Casper::Entity::StoredVersionedContractByName
    StoredVersionedContractByName serialization
  Casper::Entity::DeployExecutableTransfer
    DeployExecutableTransfer serialization

DeployHeaderSerializer
  should serialize DeployHeader

DeployNamedArgSerializer
  #to_bytes
    when DeployNamedArg has CLu32 value
      should serialize DeployNamedArg with CLu32 value
    when DeployNamedArg has CLString value
      should serialize DeployNamedArg with CLString value
    when DeployNamedArg has CLURef value
      should serialize DeployNamedArg with CLURef value
    when DeployNamedArg has CLPublicKey value
      should serialize DeployNamedArg with CLPublicKey value

DeploySerializer
  should serialize Deploy

Casper::RpcClient
  fails, wrong ip format :  65.21.0.X
  fails, 65.21.0.0 is not available in network
  #info_get_peers
    Peers Array
      passes, peers array is not nil
      passes, peers array is not empty
      passes, peers object is a type of Array
      passes, peers member are types of Hash
      passes, peer members are types of String
      passes, length of first_item equal 14
      passes, peer includes node_id key
      passes, peer includes address key
    When called info_get_peers with invalid ip address
      fails,  "SocketError"
  #chain_get_StateRootHash
    Without a block_hash parameter
      passes,  current state_root_hash is a type of String
      passes,  current state_root_hash is not nil
      passes,  current state_root_hash is not empty
      passes,  current state_root_hash is 64 characters long
    With a block_hash parameter
      passes,  current state_root_hash is a type of String
      passes,  current state_root_hash is not nil
      passes,  current state_root_hash is not empty
      passes,  current state_root_hash is 64 characters long
  #info_get_deploy
    When info_get_deploy method is called with deploy hash parameter
      passes, Deploy type is a Hash
      passes, hash value of Deploy is equal to the deploy_hash value
      passes, header is not nil
      passes, payment is not nil
      passes, payment includes ModuleBytes key
      passes, session is not nil
      passes, session includes StoredContractByHash key
      passes, approvals is not nil
      passes, approvals includes signer
      passes, approvals includes signature
    When info_get_deploy is called with an empty deploy hash parameter
      fails,  ServerError: Invalid params
    When info_get_deploy is called with an invalid parameter
      fails,  ServerError: Invalid params
      fails,  ServerError: Invalid params
  #info_get_status
    Returns the current status of the node
      passes, node includes api_version, chainspec_name, starting_state_root_hash, peers, last_added_block_info, our_public_signing_key, round_length, next_upgrade, build_version, uptime keys
      passes, network is casper
      passes, last added block includes hash, timestamp, era_id, height, state_root_hash, creator keys
      passes, the number of peers are equal
      passes, node public key is : 014382d46e2543ab2832c04936f8c205847040426abb56065bbf7b2f7e1d33f200
  #chain_get_block_transfers
    Returns all transfers for a Block from the network
      passes, transfers is not empty and the number of transfers is 2
      passes, amount of the first transaction is 6000000000000 motes
      passes, amount of the second transaction is 3997300000000 motes
      passes, all keys in transfers are 'deploy_hash', 'from', 'to',
      'source', 'target', 'amount', 'gas', 'id' respectively
  #chain_get_block
    Returns a Block from the network
      When chain_get_block method is called with deploy hash parameter
        passes, block hash : 5fdbdf3fa70d37821aa2d1752743e9653befc15e65e40c2655e1ce93a807260f
        passes, hash value of block is equal to the block hash given as parameter
        passes, block includes 'hash', 'header', 'body' and 'proofs' respectively
        passes, header includes 'parent_hash', 'state_root_hash', 'body_hash', 'random_bit',
        'accumulated_seed', 'era_end', 'timestamp', 'era_id', 'height', 'protocol_version' keys respectively
        passes, body includes 'proposer', 'deploy_hashes' and 'transfer_hashes' keys respectively
        includes public_key and signature keys
  #chain_get_eraInfo_by_SwitchBlock
    Returns an EraInfo from the network
      checks whether era_ids are equal or not
      checks whether state_root_hashes are equal or not
  #state_get_item
    Returns a stored value from the network
      checks validator_public_key equality
      checks staked_amount which is 208330980103513
      includes initial_release_timestamp_millis keys
  #state_get_dictionary_item
    checks that CLValue should not be nil
    checks that cl_type should equal to String
    checks that CLValue parsed equals to "https://caspercommunity.io"
  #state_get_balance
    is equal to 29269647684075
  #state_get_AuctionInfo
    checks state root hash equality and they should be equal
    checks that era_validators is not empty

Casper::RpcClient
  fails, wrong ip format :  65.21.0.X
  fails, 65.21.0.0 is not available in network
  #info_get_peers
    Peers Array
      passes, peers array is not nil
      passes, peers array is not empty
      passes, peers object is a type of Array
      passes, peers member are types of Hash
      passes, peer members are types of String
      passes, length of first_item equal 14
      passes, peer includes node_id key
      passes, peer includes address key
    When called info_get_peers with invalid ip address
      fails,  "SocketError"
  #chain_get_StateRootHash
    Without a block_hash parameter
      passes,  current state_root_hash is a type of String
      passes,  current state_root_hash is not nil
      passes,  current state_root_hash is not empty
      passes,  current state_root_hash is 64 characters long
    With a block_hash parameter
      passes,  current state_root_hash is a type of String
      passes,  current state_root_hash is not nil
      passes,  current state_root_hash is not empty
      passes,  current state_root_hash is 64 characters long
  #info_get_deploy
    When info_get_deploy method is called with deploy hash parameter
      passes, Deploy type is a Hash
      passes, hash value of Deploy is equal to the deploy_hash value
      passes, header is not nil
      passes, payment is not nil
      passes, payment includes ModuleBytes key
      passes, session is not nil
      passes, session includes StoredContractByHash key
      passes, approvals is not nil
      passes, approvals includes signer
      passes, approvals includes signature
    When info_get_deploy is called with an empty deploy hash parameter
      fails,  ServerError: Invalid params
    When info_get_deploy is called with an invalid parameter
      fails,  ServerError: Invalid params
      fails,  ServerError: Invalid params
  #info_get_status
    Returns the current status of the node
      passes, node includes api_version, chainspec_name, starting_state_root_hash, peers, last_added_block_info, our_public_signing_key, round_length, next_upgrade, build_version, uptime keys
      passes, network is casper
      passes, last added block includes hash, timestamp, era_id, height, state_root_hash, creator keys
      passes, the number of peers are equal
      passes, node public key is : 01ac58a7b87cd67f03b1ccf371a1f3979efb6ddafb9fbb7b59096ed5a6425eccc3
  #chain_get_block_transfers
    Returns all transfers for a Block from the network
      passes, transfers is not empty and the number of transfers is 1
      passes, all keys in transfers are 'deploy_hash', 'from', 'to',
      'source', 'target', 'amount', 'gas', 'id' respectively
      passes, amount of the first transaction is 100000000000 motes
      passes, amount of the second transaction is 120000000000 motes
  #chain_get_block
    Returns a Block from the network
      When chain_get_block method is called with deploy hash parameter
        passes, block hash : 7e89d689b1604280e1c4c83c743f58ecef1f2177f5307580313122ab11595f4b
        passes, hash value of block is equal to the block hash given as parameter
        passes, block includes 'hash', 'header', 'body' and 'proofs' respectively
        passes, header includes 'parent_hash', 'state_root_hash', 'body_hash', 'random_bit',
        'accumulated_seed', 'era_end', 'timestamp', 'era_id', 'height', 'protocol_version' keys respectively
        passes, body includes 'proposer', 'deploy_hashes' and 'transfer_hashes' keys respectively
        includes public_key and signature keys
  #chain_get_eraInfo_by_SwitchBlock
    Returns an EraInfo from the network
      passes, era_ids are equal
      passes, state_root_hashes are equal
  #state_get_item
    Returns a stored value from the network
      passes, Account includes account_hash, named_keys, main_purse, associated_keys, action_thresholds keys
      passes, account hash = account-hash-b0032b1c87261c9a440705762876a64354d37a2c57be269bae69bb450e6b8c2b
      passes, main_purse is not nil
      passes, main_purse : uref-f4d4d840464dd8934fcca9758d64cb514f52285ae0b79d706436f2cfe87e34fd-007
      passes, named_keys is not empty
      passes, deployment of action_thresholds is equal to 1
      passes, weight of associated keys is equal to 1
  #state_get_dictionary_item
    checks that CLValue should not be nil
    checks that cl_type should equal to String
    checks that CLValue parsed equals to "abc_value"
  #state_get_balance
    is equal to 390000000000
  #state_get_AuctionInfo
    checks state root hash equality and they should be equal
    checks that era_validators is not empty

Utils::TimeUtils
  serialize 1603994401469 ms to 0xbd3a847575010000
  should convert iso datetime to ms from unix epoch
  should convert miliseconds to iso datetime
  should convert ttl to milliseconds
  should convert milliseconds to ttl

Finished in 0.41166 seconds (files took 3.68 seconds to load)
238 examples, 0 failures
```

```console
Fetching https://github.com/leif-ibsen/SwiftECC from cache
Fetching https://github.com/leif-ibsen/BigInt from cache
Fetching https://github.com/leif-ibsen/ASN1 from cache
Fetched https://github.com/leif-ibsen/SwiftECC (0.79s)
Fetched https://github.com/leif-ibsen/BigInt (0.79s)
Fetched https://github.com/leif-ibsen/ASN1 (0.79s)
Fetching https://github.com/tesseract-one/Blake2.swift.git from cache
Fetched https://github.com/tesseract-one/Blake2.swift.git (0.38s)
Computing version for https://github.com/leif-ibsen/SwiftECC
Computed https://github.com/leif-ibsen/SwiftECC at 2.2.0 (0.63s)
Computing version for https://github.com/tesseract-one/Blake2.swift.git
Computed https://github.com/tesseract-one/Blake2.swift.git at 0.1.2 (0.64s)
Computing version for https://github.com/leif-ibsen/BigInt
Computed https://github.com/leif-ibsen/BigInt at 1.2.12 (0.66s)
Computing version for https://github.com/leif-ibsen/ASN1
Computed https://github.com/leif-ibsen/ASN1 at 2.0.1 (0.63s)
Creating working copy for https://github.com/tesseract-one/Blake2.swift.git
Working copy of https://github.com/tesseract-one/Blake2.swift.git resolved at 0.1.2
Creating working copy for https://github.com/leif-ibsen/ASN1
Working copy of https://github.com/leif-ibsen/ASN1 resolved at 2.0.1
Creating working copy for https://github.com/leif-ibsen/BigInt
Working copy of https://github.com/leif-ibsen/BigInt resolved at 1.2.12
Creating working copy for https://github.com/leif-ibsen/SwiftECC
Working copy of https://github.com/leif-ibsen/SwiftECC resolved at 2.2.0
[1/14] Compiling CBlake2 blake2s-ref.c
[2/14] Compiling CBlake2 blake2bp-ref.c
[3/14] Compiling CBlake2 blake2xb-ref.c
[4/14] Compiling CBlake2 blake2b-ref.c
[5/14] Compiling CBlake2 blake2xs-ref.c
[6/14] Compiling CBlake2 blake2sp-ref.c
[7/21] Compiling BigInt Limbs.swift
[8/21] Compiling BigInt FFT.swift
[9/21] Compiling BigInt BurnikelZiegler.swift
[10/21] Compiling BigInt ToomCook.swift
[11/21] Compiling BigInt BitSieve.swift
[12/21] Compiling BigInt Karatsuba.swift
[13/21] Compiling BigInt ExpMod.swift
[14/21] Compiling Blake2 Blake2.swift
[15/21] Compiling Blake2 Blake2s.swift
[16/21] Compiling Blake2 Blake2b.swift
[17/21] Compiling Blake2 Blake2xb.swift
[18/21] Compiling Blake2 Blake2sp.swift
[19/21] Compiling Blake2 Blake2bp.swift
[20/21] Compiling Blake2 Blake2xs.swift
[21/22] Merging module Blake2
[22/22] Compiling BigInt BigInt.swift
[23/23] Merging module BigInt
[24/45] Compiling ASN1 ASN1SimpleType.swift
[25/45] Compiling ASN1 ASN1T61String.swift
[26/45] Compiling ASN1 ASN1UTF8String.swift
[27/45] Compiling ASN1 InputStream.swift
[28/45] Compiling ASN1 ASN1Time.swift
[29/45] Compiling ASN1 ASN1UTCTime.swift
[30/45] Compiling ASN1 ASN1OctetString.swift
[31/45] Compiling ASN1 ASN1PrintableString.swift
[32/45] Compiling ASN1 ASN1Sequence.swift
[33/45] Compiling ASN1 ASN1Set.swift
[34/45] Compiling ASN1 ASN1Exception.swift
[35/45] Compiling ASN1 ASN1GeneralizedTime.swift
[36/45] Compiling ASN1 ASN1IA5String.swift
[37/45] Compiling ASN1 ASN1Integer.swift
[38/45] Compiling ASN1 ASN1Collection.swift
[39/45] Compiling ASN1 ASN1Ctx.swift
[40/45] Compiling ASN1 ASN1Null.swift
[41/45] Compiling ASN1 ASN1ObjectIdentifier.swift
[42/45] Compiling ASN1 ASN1BitString.swift
[43/45] Compiling ASN1 ASN1Boolean.swift
[44/45] Compiling ASN1 ASN1.swift
[45/45] Compiling ASN1 ASN1BMPString.swift
[46/46] Merging module ASN1
[47/88] Compiling SwiftECC BP192.swift
[48/88] Compiling SwiftECC BP224.swift
[49/88] Compiling SwiftECC BP256.swift
[50/88] Compiling SwiftECC EC256.swift
[51/88] Compiling SwiftECC EC384.swift
[52/88] Compiling SwiftECC EC521.swift
[53/88] Compiling SwiftECC BP320.swift
[54/88] Compiling SwiftECC BP384.swift
[55/88] Compiling SwiftECC BP512.swift
[56/88] Compiling SwiftECC Exception.swift
[57/88] Compiling SwiftECC Point.swift
[58/88] Compiling SwiftECC PrivateKey.swift
[59/88] Compiling SwiftECC DomainP.swift
[60/88] Compiling SwiftECC EC192.swift
[61/88] Compiling SwiftECC EC224.swift
[62/88] Compiling SwiftECC PublicKey.swift
[63/88] Compiling SwiftECC RP.swift
[64/88] Compiling SwiftECC Signature.swift
[65/88] Compiling SwiftECC SHA2.swift
[66/88] Compiling SwiftECC Curve.swift
[67/88] Compiling SwiftECC Domain.swift
[68/88] Compiling SwiftECC BitVector.swift
[69/88] Compiling SwiftECC EC409.swift
[70/88] Compiling SwiftECC EC571.swift
[71/88] Compiling SwiftECC Point2.swift
[72/88] Compiling SwiftECC BP160.swift
[73/88] Compiling SwiftECC Domain2.swift
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:196:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Integer(BInt(self.rp.k1)))
                     ^  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:198:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Sequence()
                     ^  ~~~~~~~~~~~~~~~
[74/88] Compiling SwiftECC EC163.swift
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:196:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Integer(BInt(self.rp.k1)))
                     ^  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:198:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Sequence()
                     ^  ~~~~~~~~~~~~~~~
[75/88] Compiling SwiftECC EC233.swift
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:196:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Integer(BInt(self.rp.k1)))
                     ^  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:198:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Sequence()
                     ^  ~~~~~~~~~~~~~~~
[76/88] Compiling SwiftECC EC283.swift
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:196:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Integer(BInt(self.rp.k1)))
                     ^  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/.build/checkouts/SwiftECC/Sources/SwiftECC/Domain2/Domain2.swift:198:22: warning: result of call to 'add' is unused
                seq1.add(ASN1Sequence()
                     ^  ~~~~~~~~~~~~~~~
[77/88] Compiling SwiftECC GCMCipher.swift
[78/88] Compiling SwiftECC HMAC.swift
[79/88] Compiling SwiftECC MD.swift
[80/88] Compiling SwiftECC OFBCipher.swift
[81/88] Compiling SwiftECC CTRCipher.swift
[82/88] Compiling SwiftECC Cipher.swift
[83/88] Compiling SwiftECC DeterministicK.swift
[84/88] Compiling SwiftECC ECBCipher.swift
[85/88] Compiling SwiftECC Base64.swift
[86/88] Compiling SwiftECC AES.swift
[87/88] Compiling SwiftECC CBCCipher.swift
[88/88] Compiling SwiftECC CFBCipher.swift
[89/89] Merging module SwiftECC
[90/188] Compiling CasperSDKInSwift CasperSDK.swift
[91/188] Compiling CasperSDKInSwift GetBlock.swift
[92/188] Compiling CasperSDKInSwift GetBlockResult.swift
[93/188] Compiling CasperSDKInSwift GetBlockTransfers.swift
[94/188] Compiling CasperSDKInSwift GetBlockTransfersParams.swift
[95/188] Compiling CasperSDKInSwift GetBlockTransfersResult.swift
[96/188] Compiling CasperSDKInSwift GetEraInfoBySwitchBlock.swift
[97/188] Compiling CasperSDKInSwift GetEraInfoResult.swift
[98/188] Compiling CasperSDKInSwift GetStateRootHash.swift
[99/188] Compiling CasperSDKInSwift JsonExecutionResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[100/188] Compiling CasperSDKInSwift OpKind.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[101/188] Compiling CasperSDKInSwift Operation.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[102/188] Compiling CasperSDKInSwift TransferAddr.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[103/188] Compiling CasperSDKInSwift Transform.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[104/188] Compiling CasperSDKInSwift TransformEntry.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[105/188] Compiling CasperSDKInSwift Groups.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[106/188] Compiling CasperSDKInSwift AccountHash.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:49:50: warning: conditional downcast from 'Any?' to 'AnyObject' is a bridging conversion; did you mean to use 'as'?
        if let transformType = from["transform"] as? AnyObject {
                               ~~~~~~~~~~~~~~~~~ ^~~ ~~~~~~~~~
                                                 as           ?
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:66:27: warning: value 'writeEraInfo' was defined but never used; consider replacing with boolean test
            } else if let writeEraInfo = transformType["WriteEraInfo"] as? [String:Any] {
                      ~~~~^~~~~~~~~~~~~~~
                      (                                                                ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:70:21: warning: variable 'retBid' was never mutated; consider changing to 'let' constant
                var retBid:Bid = Bid();
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:93:25: warning: immutable value 'totalDelegator' was never used; consider replacing with '_' or removing it
                    let totalDelegator : Int = delegators.count;
                        ^~~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/Transform.swift:105:21: warning: immutable value 'totalWithDraw' was never used; consider replacing with '_' or removing it
                let totalWithDraw:Int = WriteWithdraws.count;
                    ^~~~~~~~~~~~~
                    _
[107/188] Compiling CasperSDKInSwift GetBalanceResult.swift
[108/188] Compiling CasperSDKInSwift GetDictionaryItem.swift
[109/188] Compiling CasperSDKInSwift GetDictionaryItemParams.swift
[110/188] Compiling CasperSDKInSwift GetDictionaryItemResult.swift
[111/188] Compiling CasperSDKInSwift GetItem.swift
[112/188] Compiling CasperSDKInSwift GetItemParams.swift
[113/188] Compiling CasperSDKInSwift GetItemResult.swift
[114/188] Compiling CasperSDKInSwift JsonBid.swift
[115/188] Compiling CasperSDKInSwift Contract.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[116/188] Compiling CasperSDKInSwift ContractPackage.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[117/188] Compiling CasperSDKInSwift ContractVersion.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[118/188] Compiling CasperSDKInSwift Delegator.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[119/188] Compiling CasperSDKInSwift Bytes.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[120/188] Compiling CasperSDKInSwift Deploy.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[121/188] Compiling CasperSDKInSwift DeployHeader.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[122/188] Compiling CasperSDKInSwift DeployInfo.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:52:17: warning: initialization of immutable value 'jsonString' was never used; consider replacing with assignment to '_' or removing it
            let jsonString = String(data: jsonData, encoding: String.Encoding.ascii)!
            ~~~~^~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                print("Error message:\(message)")
                                       ^~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: use 'String(describing:)' to silence this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                       String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/Deploy.swift:73:40: note: provide a default value to avoid this warning
                print("Error message:\(message)")
                                       ^~~~~~~
                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Deploy/DeployInfo.swift:21:13: warning: variable 'oneDeployInfo' was never mutated; consider changing to 'let' constant
        var oneDeployInfo : DeployInfo = DeployInfo();
        ~~~ ^
        let
[123/188] Compiling CasperSDKInSwift PeerEntry.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[124/188] Compiling CasperSDKInSwift PeerMap.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[125/188] Compiling CasperSDKInSwift ProtocolVersion.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[126/188] Compiling CasperSDKInSwift RuntimeArgs.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[127/188] Compiling CasperSDKInSwift StoredValue.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[128/188] Compiling CasperSDKInSwift Transfer.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[129/188] Compiling CasperSDKInSwift URef.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[130/188] Compiling CasperSDKInSwift UnbondingPurse.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:265:17: warning: initialization of immutable value 'totalSei' was never used; consider replacing with assignment to '_' or removing it
            let totalSei = seigniorageAllocations.count;
            ~~~~^~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/StoredValue.swift:319:17: warning: initialization of immutable value 'totalDelegator' was never used; consider replacing with assignment to '_' or removing it
            let totalDelegator = delegators.count
            ~~~~^~~~~~~~~~~~~~
            _
[131/188] Compiling CasperSDKInSwift JsonBids.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[132/188] Compiling CasperSDKInSwift JsonDelegator.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[133/188] Compiling CasperSDKInSwift ClTypeHelper.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[134/188] Compiling CasperSDKInSwift CommonStruct.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[135/188] Compiling CasperSDKInSwift File.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[136/188] Compiling CasperSDKInSwift JsonConversion.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[137/188] Compiling CasperSDKInSwift ProtocolAll.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[138/188] Compiling CasperSDKInSwift Utils.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:118:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: warning: expression implicitly coerced from '[String : Any]?' to 'Any'
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: provide a default value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: force-unwrap the value to avoid this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                          !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:122:98: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            obj = ["jsonrpc":CASPER_RPC_VERSION,"id":CASPER_ID,"method":method.rawValue,"params":objParams]
                                                                                                 ^~~~~~~~~
                                                                                                           as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: warning: coercion of implicitly unwrappable value of type '[String : Any]?' to 'Any' does not unwrap optional
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:114:13: note: implicitly unwrapped var 'obj' declared here
        var obj:[String:Any]!
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: provide a default value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: force-unwrap the value to avoid this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                         !
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/JsonConversion.swift:131:71: note: explicitly cast to 'Any' with 'as Any' to silence this warning
            let jsonData = try JSONSerialization.data(withJSONObject: obj, options: .prettyPrinted)
                                                                      ^~~
                                                                          as Any
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Utils/Utils.swift:27:17: warning: initialization of immutable value 'totalMinute' was never used; consider replacing with assignment to '_' or removing it
            let totalMinute = m/miniuteInMilisecond
            ~~~~^~~~~~~~~~~
            _
[139/188] Compiling CasperSDKInSwift BlockHash.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[140/188] Compiling CasperSDKInSwift DeployHash.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[141/188] Compiling CasperSDKInSwift PublicKey.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[142/188] Compiling CasperSDKInSwift JsonEraValidators.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[143/188] Compiling CasperSDKInSwift MinimalBlockInfo.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[144/188] Compiling CasperSDKInSwift NamedCLTypeArg.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[145/188] Compiling CasperSDKInSwift NamedKey.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[146/188] Compiling CasperSDKInSwift NextUpgrade.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/JsonEraValidators.swift:19:29: warning: conditional cast from '[String : Any]' to '[String : Any]' always succeeds
        if let from1 = from as? [String:Any] {
                            ^
[147/188] Compiling CasperSDKInSwift GetStatusResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[148/188] Compiling CasperSDKInSwift CommonObjs.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[149/188] Compiling CasperSDKInSwift DeployExecutionResults.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[150/188] Compiling CasperSDKInSwift CLTypeSerializeHelper.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[151/188] Compiling CasperSDKInSwift GetAuctionInfo.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[152/188] Compiling CasperSDKInSwift GetAuctionInfoResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[153/188] Compiling CasperSDKInSwift GetBalance.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[154/188] Compiling CasperSDKInSwift GetBalanceParams.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:43:24: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .List(let cLType):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:45:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:47:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Result(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:23: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                  ~~~~^~~~~~~
                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:49:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:51:26: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
        case .Tuple1(let cLType):
                     ~~~~^~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:53:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple2(let cLType1, let cLType2):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:26: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                     ~~~~^~~~~~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:39: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                  ~~~~^~~~~~~
                                  _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:55:52: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
        case .Tuple3(let cLType1, let cLType2, let cLType3):
                                               ~~~~^~~~~~~
                                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:108:24: warning: immutable value 'string' was never used; consider replacing with '_' or removing it
        case .Unit(let string):
                   ~~~~^~~~~~
                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:469:30: warning: immutable value 'anyObject' was never used; consider replacing with '_' or removing it
        case .AnyCLValue(let anyObject):
                         ~~~~^~~~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:64:8: warning: will never be executed
       return ""
       ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Serialization/CLTypeSerializeHelper.swift:139:13: warning: will never be executed
            break
            ^
[155/188] Compiling CasperSDKInSwift Ed25519Crypto.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[156/188] Compiling CasperSDKInSwift Secp256k1Crypto.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[157/188] Compiling CasperSDKInSwift DeploySerialization.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[158/188] Compiling CasperSDKInSwift Account.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[159/188] Compiling CasperSDKInSwift ActionThresholds.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[160/188] Compiling CasperSDKInSwift AssociatedKey.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[161/188] Compiling CasperSDKInSwift AuctionState.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[162/188] Compiling CasperSDKInSwift Bid.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[163/188] Compiling CasperSDKInSwift JsonBlock.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:18:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:19:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:90:13: warning: initialization of immutable value 'bundleMain' was never used; consider replacing with assignment to '_' or removing it
        let bundleMain = Bundle.main
        ~~~~^~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Crypto/Secp256k1Crypto.swift:91:13: warning: initialization of immutable value 'bundleDoingTest' was never used; consider replacing with assignment to '_' or removing it
        let bundleDoingTest = Bundle(for: type(of: self ))
        ~~~~^~~~~~~~~~~~~~~
        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/DomainSerialization/DeploySerialization.swift:42:13: warning: variable 'headerSerialized' was never mutated; consider changing to 'let' constant
        var headerSerialized:String = DeployHeaderSerialization.serialize(from: fromDeployHeader)
        ~~~ ^
        let
[164/188] Compiling CasperSDKInSwift Digest.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[165/188] Compiling CasperSDKInSwift DisableVersion.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[166/188] Compiling CasperSDKInSwift EntryPoint.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[167/188] Compiling CasperSDKInSwift EraSummary.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[168/188] Compiling CasperSDKInSwift ErrorHandler.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[169/188] Compiling CasperSDKInSwift ExecutableDeployItem.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[170/188] Compiling CasperSDKInSwift ExecutionEffect.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[171/188] Compiling CasperSDKInSwift ExecutionResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:23:13: warning: variable 'ret' was never used; consider replacing with '_' or removing it
        var ret:ErrorCode = .NONE
            ^~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ErrorHandler.swift:30:20: warning: value 'data' was defined but never used; consider replacing with boolean test
            if let data = result["data"] as? String {
               ~~~~^~~~~~~
               (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:44:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:49:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:74:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:79:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:103:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:108:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:136:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:141:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:169:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:174:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:189:25: warning: variable 'runtimeArg' was never mutated; consider changing to 'let' constant
                    var runtimeArg:NamedArg = NamedArg();
                    ~~~ ^
                    let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/ExecutableDeployItem.swift:194:29: warning: variable 'value' was never mutated; consider changing to 'let' constant
                        var value:CLValue = NamedArg.jsonToCLValue(input: arg1);
                        ~~~ ^
                        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionEffect.swift:20:17: warning: initialization of immutable value 'totalOperations' was never used; consider replacing with assignment to '_' or removing it
            let totalOperations = oJsons.count
            ~~~~^~~~~~~~~~~~~~~
            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Execution/ExecutionResult.swift:23:13: warning: variable 'retExecutionResult' was never mutated; consider changing to 'let' constant
        var retExecutionResult:ExecutionResult = .None
        ~~~ ^
        let
[172/188] Compiling CasperSDKInSwift JsonBlockBody.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[173/188] Compiling CasperSDKInSwift JsonBlockHeader.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[174/188] Compiling CasperSDKInSwift JsonEraEnd.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[175/188] Compiling CasperSDKInSwift JsonEraReport.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[176/188] Compiling CasperSDKInSwift JsonProof.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[177/188] Compiling CasperSDKInSwift Reward.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[178/188] Compiling CasperSDKInSwift ValidatorWeight.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[179/188] Compiling CasperSDKInSwift CLType.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[180/188] Compiling CasperSDKInSwift CLValue.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/Block/JsonBlockHeader.swift:74:25: warning: initialization of immutable value 'totalRewards' was never used; consider replacing with assignment to '_' or removing it
                    let totalRewards = rewards.count;
                    ~~~~^~~~~~~~~~~~
                    _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:59:13: warning: variable 'clType' was never mutated; consider changing to 'let' constant
        var clType : CLType = .NONE
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:61:16: warning: value 'boolCLType' was defined but never used; consider replacing with boolean test
        if let boolCLType = from["Bool"] as? Bool {
           ~~~~^~~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:64:16: warning: value 'u8CLType' was defined but never used; consider replacing with boolean test
        if let u8CLType = from["U8"] as? UInt8 {
           ~~~~^~~~~~~~~~~
           (                                  ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:67:16: warning: value 'u32CLType' was defined but never used; consider replacing with boolean test
        if let u32CLType = from["U32"] as? UInt32 {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:73:16: warning: value 'u128CLType' was defined but never used; consider replacing with boolean test
        if let u128CLType = from["U128"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:76:16: warning: value 'u256CLType' was defined but never used; consider replacing with boolean test
        if let u256CLType = from["U256"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:79:16: warning: value 'u512CLType' was defined but never used; consider replacing with boolean test
        if let u512CLType = from["U512"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:82:16: warning: value 'stringCLType' was defined but never used; consider replacing with boolean test
        if let stringCLType = from["String"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                           ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:85:16: warning: value 'keyMapCLType' was defined but never used; consider replacing with boolean test
        if let keyMapCLType = from["key"] as? String {
           ~~~~^~~~~~~~~~~~~~~
           (                                        ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:88:16: warning: value 'valueMapCLType' was defined but never used; consider replacing with boolean test
        if let valueMapCLType = from["value"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~
           (                                            ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:91:16: warning: value 'okResult' was defined but never used; consider replacing with boolean test
        if let okResult = from["ok"] as? String {
           ~~~~^~~~~~~~~~~
           (                                   ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:94:16: warning: value 'errResult' was defined but never used; consider replacing with boolean test
        if let errResult = from["err"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:100:16: warning: value 'keyCLType' was defined but never used; consider replacing with boolean test
        if let keyCLType = from["Key"] as? String {
           ~~~~^~~~~~~~~~~~
           (                                     ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:103:16: warning: value 'publicKeyCLType' was defined but never used; consider replacing with boolean test
        if let publicKeyCLType = from["PublicKey"] as? String {
           ~~~~^~~~~~~~~~~~~~~~~~
           (                                                 ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:106:16: warning: value 'URefClType' was defined but never used; consider replacing with boolean test
        if let URefClType = from["URef"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:109:16: warning: value 'UnitCLType' was defined but never used; consider replacing with boolean test
        if let UnitCLType = from["Unit"] as? String {
           ~~~~^~~~~~~~~~~~~
           (                                       ) != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:170:31: warning: cast from '[AnyObject]' to unrelated type 'NSNull' always fails
            if !(tuple3CLType is NSNull) {
                 ~~~~~~~~~~~~ ^  ~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:145:17: warning: variable 'counter' was never mutated; consider changing to 'let' constant
            var counter : Int = 0;
            ~~~ ^
            let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLType.swift:220:42: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        else if let clTypeWrapper = from as? AnyObject {
                                         ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:58:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Result(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:64:28: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .List(let cLType):
                       ~~~~^~~~~~
                       _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:67:33: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .FixedList(let cLType):
                            ~~~~^~~~~~
                            _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:27: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                      ~~~~^~~~~~~
                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:70:40: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Map(let cLType1, let cLType2):
                                   ~~~~^~~~~~~
                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:73:30: warning: immutable value 'cLType' was never used; consider replacing with '_' or removing it
            case .Tuple1(let cLType):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:76:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple2(let cLType1, let cLType2):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:30: warning: immutable value 'cLType1' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                         ~~~~^~~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:43: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                      ~~~~^~~~~~~
                                      _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:79:56: warning: immutable value 'cLType3' was never used; consider replacing with '_' or removing it
            case .Tuple3(let cLType1, let cLType2, let cLType3):
                                                   ~~~~^~~~~~~
                                                   _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:118:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:422:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:480:34: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
            if let parsed = from as? AnyObject {
                                 ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:481:37: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
                if parsed is NSNull != nil {
                   ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:519:30: warning: conditional cast from 'AnyObject' to 'AnyObject' always succeeds
        if let parsed = from as? AnyObject {
                             ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:520:33: warning: comparing non-optional value of type 'Bool' to 'nil' always returns true
            if parsed is NSNull != nil {
               ~~~~~~~~~~~~~~~~ ^  ~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:500:22: warning: immutable value 'key' was never used; consider replacing with '_' or removing it
                for (key,value) in parsed {
                     ^~~
                     _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:514:30: warning: immutable value 'uInt32' was never used; consider replacing with '_' or removing it
        case .BytesArray(let uInt32):
                         ~~~~^~~~~~
                         _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:586:36: warning: immutable value 'cLType2' was never used; consider replacing with '_' or removing it
        case .Map(let cLType1, let cLType2):
                               ~~~~^~~~~~~
                               _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:605:21: warning: variable 'counter' was never mutated; consider changing to 'let' constant
                var counter : Int = 0;
                ~~~ ^
                let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:127:9: warning: will never be executed
        return "";
        ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:428:13: warning: code after 'return' will never be executed
            break
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:565:13: warning: code after 'return' will never be executed
            break;
            ^
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/CLValue.swift:654:13: warning: code after 'return' will never be executed
            break
            ^
[181/188] Compiling CasperSDKInSwift VestingSchedule.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[182/188] Compiling CasperSDKInSwift HttpHandler.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[183/188] Compiling CasperSDKInSwift GetDeploy.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[184/188] Compiling CasperSDKInSwift GetDeployParams.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[185/188] Compiling CasperSDKInSwift GetDeployResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[186/188] Compiling CasperSDKInSwift GetPeers.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[187/188] Compiling CasperSDKInSwift GetPeersResult.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[188/188] Compiling CasperSDKInSwift GetStatus.swift
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Entity/VestingSchedule.swift:16:13: warning: variable 'ret' was never mutated; consider changing to 'let' constant
        var ret:VestingSchedule = VestingSchedule();
        ~~~ ^
        let
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:103:65: note: provide a default value to avoid this warning
                        NSLog("Payment:\(getDeployResult.deploy.payment)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:42: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: use 'String(describing:)' to silence this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                         String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:104:65: note: provide a default value to avoid this warning
                        NSLog("Session:\(getDeployResult.deploy.session)")
                                         ~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~
                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                    String(describing:       )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:161:83: note: provide a default value to avoid this warning
                                NSLog("First transfer deploy_hash:\(firstTransfer.deploy_hash)")
                                                                    ~~~~~~~~~~~~~~^~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:62: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ^~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                             String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:162:76: note: provide a default value to avoid this warning
                                NSLog("First transfer from:\(firstTransfer.from)")
                                                             ~~~~~~~~~~~~~~^~~~
                                                                                ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:163:74: note: provide a default value to avoid this warning
                                NSLog("First transfer to:\(firstTransfer.to)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:164:85: note: provide a default value to avoid this warning
                                NSLog("First transfer source:\(firstTransfer.source.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:64: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                               String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:165:85: note: provide a default value to avoid this warning
                                NSLog("First transfer target:\(firstTransfer.target.value)")
                                                               ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:60: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ^~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: use 'String(describing:)' to silence this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                           String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:167:74: note: provide a default value to avoid this warning
                                NSLog("First transfer id:\(firstTransfer.id)")
                                                           ~~~~~~~~~~~~~~^~
                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:67: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                  String(describing:                               )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:189:111: note: provide a default value to avoid this warning
                            NSLog("Block body first deploy hash:\(getBlockResult.block.body.deployHash.first!.value)")
                                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                    ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:69: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: use 'String(describing:)' to silence this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                    String(describing:                                 )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:193:115: note: provide a default value to avoid this warning
                            NSLog("Block body first transfer hash:\(getBlockResult.block.body.transferHash.first!.value)")
                                                                    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                                        ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:73: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: use 'String(describing:)' to silence this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                        String(describing:                    )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:238:97: note: provide a default value to avoid this warning
                        NSLog("GetDictionaryItemResult dictionary_key:\(getDictionaryItemResult.dictionary_key)")
                                                                        ~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:76: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: use 'String(describing:)' to silence this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                           String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:262:103: note: provide a default value to avoid this warning
                            NSLog("AuctionState first bid bonding_purse: \(firstBid.bid.bonding_purse.value)")
                                                                           ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                            ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: use 'String(describing:)' to silence this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:                )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:269:101: note: provide a default value to avoid this warning
                                NSLog("First delegator bonding_purse:\(firstDelegator.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                          ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:157:32: warning: value 'transfer' was defined but never used; consider replacing with boolean test
                        if let transfer = getBlockTransferResult.transfers {
                           ~~~~^~~~~~~~~~~
                                                                           != nil
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:35: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Account hash:\(account.account_hash.value)")
                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: use 'String(describing:)' to silence this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                  String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:304:56: note: provide a default value to avoid this warning
            NSLog("Account hash:\(account.account_hash.value)")
                                  ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                  String(describing:                  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:305:77: note: provide a default value to avoid this warning
            NSLog("Action threshold delployment:\(account.action_thresholds.deployment)")
                                                  ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~
                                                                                       ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:54: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: use 'String(describing:)' to silence this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                     String(describing:                      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:306:80: note: provide a default value to avoid this warning
            NSLog("Action threshold key_management:\(account.action_thresholds.key_management)")
                                                     ~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~~~~~~~~~~
                                                                                              ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:59: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ^~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                          String(describing:        )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:310:80: note: provide a default value to avoid this warning
                NSLog("First associate_key account_hash:\(firstAK.account_hash.value)")
                                                          ~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ^~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: use 'String(describing:)' to silence this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                    String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:311:61: note: provide a default value to avoid this warning
                NSLog("First associate_key weight:\(firstAK.weight)")
                                                    ~~~~~~~~^~~~~~
                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:33: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Main purse:\(account.main_purse.value)")
                                ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: use 'String(describing:)' to silence this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:313:52: note: provide a default value to avoid this warning
            NSLog("Main purse:\(account.main_purse.value)")
                                ~~~~~~~~~~~~~~~~~~~^~~~~
                                                         ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:53: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                    String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:326:62: note: provide a default value to avoid this warning
            NSLog("Contract contract_package_hash:\(contract.contract_package_hash)")
                                                    ~~~~~~~~~^~~~~~~~~~~~~~~~~~~~~
                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:50: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: use 'String(describing:)' to silence this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                 String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:327:59: note: provide a default value to avoid this warning
            NSLog("Contract contract_wasm_hash:\(contract.contract_wasm_hash)")
                                                 ~~~~~~~~~^~~~~~~~~~~~~~~~~~
                                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point name:\(firstEP.name)")
                                                ^~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:337:57: note: provide a default value to avoid this warning
                NSLog("First entry_point name:\(firstEP.name)")
                                                ~~~~~~~~^~~~
                                                             ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:61: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ^~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                            String(describing:      )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:338:69: note: provide a default value to avoid this warning
                NSLog("First entry_point entry_point_type:\(firstEP.entry_point_type)")
                                                            ~~~~~~~~^~~~~~~~~~~~~~~~
                                                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:48: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ^~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: use 'String(describing:)' to silence this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                               String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:339:56: note: provide a default value to avoid this warning
                NSLog("First entry_point ret:\(firstEP.ret)")
                                               ~~~~~~~~^~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:49: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: use 'String(describing:)' to silence this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                String(describing:              )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:345:76: note: provide a default value to avoid this warning
            NSLog("ContractPackage access_key:\(contractPackage.access_key.value)")
                                                ~~~~~~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:43: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ^~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                          String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:353:52: note: provide a default value to avoid this warning
            NSLog("Transfer deploy_hash:\(transfer.deploy_hash)")
                                          ~~~~~~~~~^~~~~~~~~~~
                                                               ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer from:\(transfer.from)")
                                   ^~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:354:45: note: provide a default value to avoid this warning
            NSLog("Transfer from:\(transfer.from)")
                                   ~~~~~~~~~^~~~
                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer source:\(transfer.source.value)")
                                     ^~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                     String(describing:   )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:355:54: note: provide a default value to avoid this warning
            NSLog("Transfer source:\(transfer.source.value)")
                                     ~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:38: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Transfer target:\(transfer.target)")
                                     ^~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: use 'String(describing:)' to silence this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                     String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:356:47: note: provide a default value to avoid this warning
            NSLog("Transfer target:\(transfer.target)")
                                     ~~~~~~~~~^~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: use 'String(describing:)' to silence this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:363:54: note: provide a default value to avoid this warning
            NSLog("Deploy source:\(deployInfo.source.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:51: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: use 'String(describing:)' to silence this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                  String(describing:            )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:374:61: note: provide a default value to avoid this warning
                    NSLog("Validator public key:\(validator.validator_public_key)")
                                                  ~~~~~~~~~~^~~~~~~~~~~~~~~~~~~~
                                                                                 ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ^~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: use 'String(describing:)' to silence this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                   String(describing:     )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:387:54: note: provide a default value to avoid this warning
            NSLog("bonding_purse:\(bid.bonding_purse.value)")
                                   ~~~~~~~~~~~~~~~~~~^~~~~
                                                           ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:36: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ^~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: use 'String(describing:)' to silence this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                   String(describing:  )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:388:40: note: provide a default value to avoid this warning
            NSLog("staked_amount:\(bid.staked_amount)")
                                   ~~~~^~~~~~~~~~~~~
                                                     ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:72: warning: string interpolation produces a debug description for an optional value; did you mean to make this explicit?
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ^~~~~~~~~~~~~~~~~~~~~~~~~~~
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: use 'String(describing:)' to silence this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                       String(describing:         )
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/HttpHandler.swift:396:94: note: provide a default value to avoid this warning
                NSLog("Withdraw first  UnbondingPurse, bonding_purse:\(firstUP.bonding_purse.value)")
                                                                       ~~~~~~~~~~~~~~~~~~~~~~^~~~~
                                                                                                   ?? <#default value#>
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetDeploy.swift:35:29: warning: initialization of immutable value 'totalApproval' was never used; consider replacing with assignment to '_' or removing it
                        let totalApproval = approvals.count
                        ~~~~^~~~~~~~~~~~~
                        _
/Users/p35862/CasperSDKInSwift/Sources/CasperSDKInSwift/Info/GetPeers.swift:15:17: warning: variable 'getPeerResult' was never mutated; consider changing to 'let' constant
            var getPeerResult:GetPeersResult = GetPeersResult();
            ~~~ ^
            let
[189/189] Merging module CasperSDKInSwift
[189/189] Build complete!
```
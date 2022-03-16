Grant Proposal | [409 - Towards Decentralized Documents: Remove LibreOffice Column Limits](https://portal.devxdao.com/public-proposals/409)
------------ | -------------
Milestone | 1
Milestone Title | XLSX import/export
OP | Muhammet Kara
Reviewer | Yusuf Keten

# Milestone Details
The review will cover the 1st milestone criteria set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestone:**

Remove the 1024 columns limit in Calc and make it dynamic: up to the  XLSX import/export.

**Acceptance criteria:**

XLSX import/export feature will be verifiable by following the steps below:

1) Create a document in Excel that has more than 1024 columns.
2) Save it as XLSX.
3) Open it in Calc.
4) Notice that the file opens without truncating the content to 1024 columns.
5) Make some changes to the file, save it to XLSX.
6) Open the resulting XLSX in Excel and confirm that no columns are truncated.

**Additional notes regarding submission from OP:**

We have finished working on the XLSX filter, and once you opt in for this
new feature, it works reasonably well for the:

Remove the 1024 columns limit in Calc and make it dynamic: up to
the XLSX import/export.

milestone.

A demo document: https://github.com/mrkara/ColumnLimitSampleDocs/raw/master/orig.xlsx

(Loading this just crashes on libreoffice-7-3 and both XLSX import and export works on master, where our work has been merged.)

Here is how you can test this yourself:

1) Get a master daily build from https://dev-builds.libreoffice.org/daily/master/current.html

2) Start LibreOffice, go to Tools -> Options -> LibreOffice -> Advanced,
enable Experimental features, and restart LibreOffice.

3) Go to Calc, then Tools -> Options -> Calc -> Defaults, enable "very
large spreadsheets".

Then close the empty Calc document and you can start testing.

Let us know if it helps to have a short screenshare session where we
show you this in action.

Opting in is necessary for now, as the "enable very large spreadsheet"
switch is a global one, and we plan to enable it during March, when ODS
support will be also ready.

Please find the list of related commits so far, below.

Thank you!

<<<
9c7f3ddf5b3c23de0fed08fa3ebdfa2a95fec588 optimize  XclExpRowBuffer::GetOrCreateRow() (tdf#140893)
131710cba68e46c175babbd20c810e7fc2fb811f optimize AreaBroadcast() a bit
725e1066cbe3bbd6759b3e7396bc5d0ecb55a504 remove MAXCOL/MAXROW from  ScAddress/ScRange (tdf#147509)
35cad9f57e761eef78820d092a4bb9d2f0641052 convert more MAXCOL/MAXROW
50a125464eb70cad42ef906d688e89881796cf38 remove MAXCOLCOUNT from calc pivot  implementation
957d99a539df6e21fd40370938ca5dab1613cf8c fix range checking in calls like  ScDocument::GetNote()
7bb0b11873d0c96d8116b327987834db048754c3 fix range checking when parsing Calc  cell address (tdf#147451)
05259e880db187f6698d6d545504775459d6e96a optimize blank cell Excel export  (tdf#133749)
855a0f40b285a438f8bd2ea61ebb8717daa16292 std::map -> std::unordered_map
af0a0777584825035dbf5ba0ec48d7a6412010c2 fix maxrow/maxcol mixup
6267a995ea5a621f5f147e5866b6af9cdd205b9c remove MAXCOL/MAXROW from  ScExternalRefCache
823eb92025853d120c17790d1c8efde59f033c69 do not allocate columns in  ScTable::GetPattern()
a717029e217621482ef799731f945090c6d6be4b for unallocated columns check default  column attributes (tdf#132057)
980b91d5c850099766bf32dfe28880df8873c046 move simple checks out of  DEBUG_COLUMN_STORAGE
069c0b32e2ca85340bc79a222bae57bef7d1f674 clamp ColumnSpanSet::executeAction()  to allocated columns
91c54829e84a372e9ea7460474a84abbef3d1171 do not allocate columns in  ScTable::GetNumberFormat()
8fc4e188586cf3c04592e0c1027a0c384bd3c54d non-const ScTable::GetFormulaCell()  doesn't need to allocate columns
d0a42ce9b1033a200f8d354c1abf8c3b0d569f46 avoid debug build failing on an  assert for tdf#144537
309f0f882b34c13d970677c2564f088c36c9691b simplify code
6283ac89d76d68b7c09e018be78ec6b31018da9c make ScBigAddress use 64bit
28cbc0dcb955954b4d9b85376f356999af429f06 move nInt32Min/nInt32Max to  ScBigRange and rename to nRangeMin/Max
4343976f0d38d727786b15a353ad3d49e76a65b8 remove harcoded MAXCOL/MAXROW from  ScBigAddress
92d08206b48f8ac426dce9bdfda599cb997e1f41 test for jumbosheet named ranges  export/import
3c24fe20ec6cb450abc4a822d323874ebbaecb10 don't export a document twice in a  test when not needed
a97a492080b0dd0a885e32e7ebb8f1b9899f889c tests for import/export of  full-row/column ranges in huge sheets
af85db89093767656382106b0ff8da68c0afecc9 finally write entire row/column  references as such to ODS
4eb0ee5032903d301c0dde30ed3d25d16cab3a4c make sanitizers happy
0691cc55148503448012326b070aa9209c54270b remove hardcoded MAXCOL/MAXROW from  datatableview.cxx (tdf#135332)
7adb3757944452a0f3a1a12fee1dd504eb90a1df don't gradually move columns to a  large distance (tdf#144380)
32e480cecd9f5c35880a8d1762012e44c36c478c remove use of MAXCOL/MAXROW from  address.hxx
8bb457d17ef970676f60976cc4e2de9c9f5340c0 dynamic logarithmic columns in ScBroadcastAreaSlotMachine
73cfd7eeac7031c97a57bba82677f36ef1eff731 avoid destructing many unique_ptr's most of which are nullptr
d48e68407931fc33044aa7f3fc9e971897fac610 clean up accessing CellInfo array in RowInfo
98d51bf8ce13bdac2d71f50f58d6d0ddb9041a4f speed up SfxItemPool searches with items that can't use IsSortable()
cf8408bfcbaca2998d47a56df9f1dc6f3cb98b0e make the large-sheet maxrow value pow2-based and not pow10-based
545622887c55e935be2bb482b838a8fb84a84298 optimize ScViewData::GetScrPos() for many hidden rows/columns
d20598d14a95675a436736679ab4a82a8cc3a703 optimize ScTabView::SkipCursorVertical() for many hidden rows
cd50d33fc4af3f2d4ab40de98ecf02f0d832d750 MAXCOL/MAXROW -> ScSheetLimits in fillinfo.cxx
03f225039b366f075b23a074e63edc6a47b12d3c if these are row/column numbers, then no need to use sal_uLong
fd4384c59eefc8f34d5fe90929d7cb44ee15b27f avoid overflows in ScFlatUInt16RowSegments
c24b04707c5b914bda22d709c2da025c784f5045 remove pointless BCA_SLOTS_ROW assertions
ff8e1199b338df5f28b200d417947c96fc919b12 basic import/export test for ods/xlsx with a value in column 2000
06759801f0a9e8ee80790cf7b8aa02fcb47290a0 rename class in jumbosheets-test.cxx to ScJumboSheetsTest
063997f8371f634e671947866b9e12e0a56c0f63 remove obsolete code (and last MAXCOL/MAXROW) from excel filter
a3510e31065245987e5314c821d5688e0d73442f remove hardcoded MAXCOL/MAXROW in ScRangeListTabs
6a6a147ecebfbc4f0c8a3d626737104155426393 move ScRangeListTabs members from RootData to XclImpRoot
5e402bac39dc4245844efbde442bdb3bd993a157 remove most hardcoded MAXCOL/MAXROW from Calc filters
8232965cfb5f50bb2e01f7749d04c227a9622860 replace various sal_uLong that might overflow with huge sheets
5b2a153779b68e8454a66973579512fe17e376d5 do not call purge() on string pool too often (tdf#125428)

Grant Portion
€ 21,343

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/LibreOffice/core | [9c7f3dd](https://github.com/LibreOffice/core/commit/9c7f3ddf5b3c23de0fed08fa3ebdfa2a95fec588)


# Install & Usage Testing Procedure and Findings

There is a guide about the build process of LibreOffice. However, all of the submission commits are merged into the project. Therefore, the reviewer installed the latest LibreOffice master build. (2022-Mar-15 14:29) The project is tested on macOS BigSur 11.4 and the installation file name was ["LibreOfficeDev_7.4.0.0.alpha0_MacOS_x86-64.dmg".](https://dev-builds.libreoffice.org/daily/master/MacOSX-x86_64@tb81-TDF/2022-03-15_15.39.42/LibreOfficeDev_7.4.0.0.alpha0_MacOS_x86-64.dmg)

Build Guideline: https://www.libreoffice.org/about-us/source-code/

Daily master builds: https://dev-builds.libreoffice.org/daily/master/

## Overall Impression of usage testing

The commits are all merged into the project. LibreOffice has a strict CI/CD process. Also, the reviewer installed the latest LibreOffice master build successfully. The reviewer has observed that it can open any document that has more than 1024 columns. Lastly, the reviewer has observed that the document can be saved and opened in Excel without any truncation.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

LibreOffice has two types of automatic checks:
* unit tests check low level functionality at compile time
* subsequenttests check high level functionality

The build output includes the unit tests that run at compile time. After the last commit is pushed to the repository, the CI tool has started a build with tests. The build has finished successfully.

Build Link: https://ci.libreoffice.org/job/gerrit_master/108563/

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS

# Documentation

### Code Documentation

A sufficient amount of low-level documentation exists on the project via properly formatted inline comments on the critical classes and the methods.

Requirement | Finding
------------ | -------------
Code Documented | PASS

### Project Documentation

LibreOffice has a well-defined documentation structure. There is a wiki page for developers and a wiki page for users.

LibreOffice TDF Wiki: https://wiki.documentfoundation.org/Main_Page

Requirement | Finding
------------ | -------------
Usage Documented | PASS
Example Documented | PASS

## Overall Conclusion on Documentation
Based on the reviewer's findings, this review should pass.

# Open Source Practices

## Licenses

The base repository is correctly released under the GNU GPL License.

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS

## Contribution Policies

Pull requests and issues are enabled on the repositories. LibreOffice has a [security policy.](https://www.libreoffice.org/about-us/security/) Also, the project has a detailed [contribution guide.](https://wiki.documentfoundation.org/Development)

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS

# Coding Standards

## General Observations

All of the commits are readable and well-structured. Also, they are appropriate for LibreOffice code standards. The commits are well-commented.

# Final Conclusion

LibreOffice has a high quality CI/CD pipeline. Also, the LibreOffice developer community has a high quality code review process. Therefore, the project provides the functionality that is required by the project. Also, it meets the acceptance criteria. Thus, in the reviewer's opinion, this submission should pass.

# Recommendation

Recommendation | PASS
------------ | -------------

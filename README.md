# CBT433
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. 
Due to amazing work by Alison Zhang and Jake Choi repos are no longer deleted.

```
//***FILE 433 is by Frank Clarke and contains a collection of his   *   FILE 433
//*           REXX execs.                                           *   FILE 433
//*                                                                 *   FILE 433
//*           email:  Frank Clarke <rexxhead@yahoo.com>             *   FILE 433
//*                                                                 *   FILE 433
//*         A few obsolete routines have been dropped from the      *   FILE 433
//*         prior package.  A few are not my work, but are needed   *   FILE 433
//*         as external routines by members here.                   *   FILE 433
//*                                                                 *   FILE 433
//*               'FCLARKE.TOOLPACK.EXEC' - Directory               *   FILE 433
//*                                                                 *   FILE 433
//*                 Usage or                                        *   FILE 433
//*       Member    Caller      Description                         *   FILE 433
//*       ========  =========   =================================   *   FILE 433
//*                                                                 *   FILE 433
//*       $EXAMPLE  fragment    Pro-forma new paragraph             *   FILE 433
//*                                                                 *   FILE 433
//*       @@README  text        About the material in this          *   FILE 433
//*                             library                             *   FILE 433
//*                                                                 *   FILE 433
//*       @FILE433  text        Inventory                           *   FILE 433
//*                                                                 *   FILE 433
//*       ACQ       exec        Copy a member to the 1st dataset    *   FILE 433
//*                             of a file                           *   FILE 433
//*                                                                 *   FILE 433
//*       ADDCMDS   exec        Apply TMPCMDS to ISPCMDS            *   FILE 433
//*                                                                 *   FILE 433
//*       ALIST     exec        Display current allocations         *   FILE 433
//*                                                                 *   FILE 433
//*       ATTACH    exec        Logon customization                 *   FILE 433
//*                                                                 *   FILE 433
//*       BLOX      exec        Block letter write modeled after    *   FILE 433
//*                             IEFSD095                            *   FILE 433
//*                                                                 *   FILE 433
//*       CMDUPD    exec        Update local command table          *   FILE 433
//*                                                                 *   FILE 433
//*       COMBINE   exec        Combine 2 or more datasets with     *   FILE 433
//*                             incompat DCBs                       *   FILE 433
//*                                                                 *   FILE 433
//*       COMMANDS  exec        Display current command table       *   FILE 433
//*                             contents                            *   FILE 433
//*                                                                 *   FILE 433
//*       DEIMBED   fragment    Extract ISPF elements from REXX     *   FILE 433
//*                                                                 *   FILE 433
//*       DFLTTLIB  fragment    How to set up a default ISPTLIB     *   FILE 433
//*                                                                 *   FILE 433
//*       DIRSTATS  exec        LISTD with statistics               *   FILE 433
//*                                                                 *   FILE 433
//*       DSPROF    exec        Display via LISTDSI dataset         *   FILE 433
//*                             characteristics                     *   FILE 433
//*                                                                 *   FILE 433
//*       DSVCSI    exec        Catalog Search Interface            *   FILE 433
//*                                                                 *   FILE 433
//*       DUP       exec        Allocate or copy-to a new dataset   *   FILE 433
//*                                                                 *   FILE 433
//*       EDBR      macro       Edit-from-Browse                    *   FILE 433
//*                                                                 *   FILE 433
//*       FCCMDUPD  exec        Insert a new command onto TMPCMDS   *   FILE 433
//*                                                                 *   FILE 433
//*       FCXREF    exec        Cross-reference 2 or more PDSs      *   FILE 433
//*                                                                 *   FILE 433
//*       FIRSTIME  exec        Control re-runs                     *   FILE 433
//*                                                                 *   FILE 433
//*       FIXSTATS  exec        Manipulate ISPF member stats        *   FILE 433
//*                                                                 *   FILE 433
//*       FIXTBL    exec        Jump to ISPF 3.9                    *   FILE 433
//*                                                                 *   FILE 433
//*       FLTTBL    exec        Flatten any table (see RSTTBL)      *   FILE 433
//*                                                                 *   FILE 433
//*       FSMSG     exec        Send a multi-line message           *   FILE 433
//*                                                                 *   FILE 433
//*       GENCARD   exec        Produce control card from parms     *   FILE 433
//*                                                                 *   FILE 433
//*       GETIA     macro       Extract Impact Analysis from        *   FILE 433
//*                             REXXSKEL-based code                 *   FILE 433
//*                                                                 *   FILE 433
//*       ICEUSER   exec        Authorized users                    *   FILE 433
//*                                                                 *   FILE 433
//*       IDENT     macro       Insert membername to REXX code      *   FILE 433
//*                                                                 *   FILE 433
//*       ISOLATE   macro       ONLY this word                      *   FILE 433
//*                                                                 *   FILE 433
//*       JFORM     macro       Reformat JCL                        *   FILE 433
//*                                                                 *   FILE 433
//*       JOBCARDS  exec        Build/update default jobcards       *   FILE 433
//*                             for JCL                             *   FILE 433
//*                                                                 *   FILE 433
//*       KED       macro       Edit DDN(mbr); aliased as KBR       *   FILE 433
//*                             and KVW                             *   FILE 433
//*                                                                 *   FILE 433
//*       LA        exec        LISTA ST to a scrollable display    *   FILE 433
//*                                                                 *   FILE 433
//*       LDOW      exec        Calc nth-day-of-the-week for any    *   FILE 433
//*                             month                               *   FILE 433
//*                                                                 *   FILE 433
//*       LISTCSUM  exec        LISTCAT subroutine for VCX          *   FILE 433
//*                                                                 *   FILE 433
//*       LOADKEYS  exec        Key definitions                     *   FILE 433
//*                                                                 *   FILE 433
//*       MAKEPARA  macro       Generate new paragraph for          *   FILE 433
//*                             REXXSKEL-based code                 *   FILE 433
//*                                                                 *   FILE 433
//*       MDEL      exec        Delete a member from anywhere       *   FILE 433
//*                                                                 *   FILE 433
//*       MEMBERS   exec        Return memberlist to the stack      *   FILE 433
//*                                                                 *   FILE 433
//*       MEMIDX    exec        Create/Update #INDEX (this          *   FILE 433
//*                             member)                             *   FILE 433
//*                                                                 *   FILE 433
//*       MIGRATE   exec        Migrate code from work to final     *   FILE 433
//*                                                                 *   FILE 433
//*       MREN      exec        Rename a member from anywhere       *   FILE 433
//*                                                                 *   FILE 433
//*       MTHLIM    SCHED       Determine Start-DOW and length      *   FILE 433
//*                             of a month                          *   FILE 433
//*                                                                 *   FILE 433
//*       NOOP      exec        IEFBR14                             *   FILE 433
//*                                                                 *   FILE 433
//*       OUTDENTS  macro       Show only do-end etc.               *   FILE 433
//*                                                                 *   FILE 433
//*       PACKING   fragment    How to convert to/from FIXED        *   FILE 433
//*                             DECIMAL                             *   FILE 433
//*                                                                 *   FILE 433
//*       PDSCOPYD  exec        Copy a member with stats            *   FILE 433
//*                                                                 *   FILE 433
//*       PDS2SEQ   exec        Convert PDS to IEBGENER input       *   FILE 433
//*                                                                 *   FILE 433
//*       PERMCLAS  fragment    Supply STGCLASS and MGMTCLASS       *   FILE 433
//*                                                                 *   FILE 433
//*       POPINDX   exec        Populate one #INDEX member from     *   FILE 433
//*                             another                             *   FILE 433
//*                                                                 *   FILE 433
//*       POSIT     macro       Position an Edit/View session       *   FILE 433
//*                                                                 *   FILE 433
//*       PROFILES  exec        Manipulate Edit profiles            *   FILE 433
//*                                                                 *   FILE 433
//*       PROFVARS  exec        Display variables in profiles       *   FILE 433
//*                                                                 *   FILE 433
//*       QPWEXP    exec        When does my password expire?       *   FILE 433
//*                                                                 *   FILE 433
//*       REALIAS   exec        Re-establish aliases from the       *   FILE 433
//*                             Impact Analysis                     *   FILE 433
//*                                                                 *   FILE 433
//*       REXXIA    exec        Do an Impact Analysis for an        *   FILE 433
//*                             entire dataset                      *   FILE 433
//*                                                                 *   FILE 433
//*       REXXSKEL  example     Basis for most code here            *   FILE 433
//*                                                                 *   FILE 433
//*       RSTTBL    exec        Restore a table flattened by        *   FILE 433
//*                             FLTTBL                              *   FILE 433
//*                                                                 *   FILE 433
//*       RUNDATA   exec        Maintain application-specific       *   FILE 433
//*                             information                         *   FILE 433
//*                                                                 *   FILE 433
//*       SAYVAR    exec        Display/Update variables from       *   FILE 433
//*                             ISPF pools                          *   FILE 433
//*                                                                 *   FILE 433
//*       SCHED     exec        Create a calendar page for one      *   FILE 433
//*                             month                               *   FILE 433
//*                                                                 *   FILE 433
//*       SCRAM     exec        Produce FTP files for               *   FILE 433
//*                             transferring libraries              *   FILE 433
//*                                                                 *   FILE 433
//*       SEIZE     exec        Copy a member to a distant          *   FILE 433
//*                             dataset with stats                  *   FILE 433
//*                                                                 *   FILE 433
//*       SELMATCH  macro       Match )SEL and )ENDSEL in           *   FILE 433
//*                             skeleton                            *   FILE 433
//*                                                                 *   FILE 433
//*       SEQ2PDS   exec        Anti-process of PDS2SEQ             *   FILE 433
//*                                                                 *   FILE 433
//*       SETALIAS  exec        Establish dataset aliases           *   FILE 433
//*                                                                 *   FILE 433
//*       SETEPROF  macro       Set ZDEFAULT profile                *   FILE 433
//*                                                                 *   FILE 433
//*       SETREFS   macro       Change JCL DSNs to                  *   FILE 433
//*                             backward-references                 *   FILE 433
//*                                                                 *   FILE 433
//*       SHORTRX   fragment    No-frills REXX-base                 *   FILE 433
//*                                                                 *   FILE 433
//*       SHOWFLOW  macro       Display CALLs and targets in REXX   *   FILE 433
//*                                                                 *   FILE 433
//*       SHOWME    exec        Display first-found by DDName       *   FILE 433
//*                                                                 *   FILE 433
//*       SORTCMDS  exec        Sort a Command Table                *   FILE 433
//*                                                                 *   FILE 433
//*       SQRT      exec        Square root (claimed by Robin       *   FILE 433
//*                             Ryerse)                             *   FILE 433
//*                                                                 *   FILE 433
//*       STAKEDIT  exec        Recursive Edit/Browse/View          *   FILE 433
//*                             (ED/BR/VW)                          *   FILE 433
//*                                                                 *   FILE 433
//*       STEPS     macro       Bring out all JCL EXEC rows         *   FILE 433
//*                                                                 *   FILE 433
//*       STRLEN    macro       Display a length-line over a        *   FILE 433
//*                             quoted string                       *   FILE 433
//*                                                                 *   FILE 433
//*       STRSORT   exec        Sort a string of words              *   FILE 433
//*                                                                 *   FILE 433
//*       SUPBR     exec        SuperBrowse                         *   FILE 433
//*                                                                 *   FILE 433
//*       SUPED     exec        SuperEdit                           *   FILE 433
//*                                                                 *   FILE 433
//*       SYSAMON   exec        Groom/Report activity in SYSUMON    *   FILE 433
//*                                                                 *   FILE 433
//*       SYSUMON   exec        Count tool usage                    *   FILE 433
//*                                                                 *   FILE 433
//*       SYSVARS   exec        Show SYSVARs and MVSVARs            *   FILE 433
//*                                                                 *   FILE 433
//*       S2PTRIM   subr        Subr of SEQ2PDS                     *   FILE 433
//*                                                                 *   FILE 433
//*       TBCOPY    exec        Copy a table using AAMSTR           *   FILE 433
//*                                                                 *   FILE 433
//*       TBLGEN    exec        Build a table from AAMSTR specs     *   FILE 433
//*                                                                 *   FILE 433
//*       TBLMSTR   exec        Maintain AAMSTR table               *   FILE 433
//*                                                                 *   FILE 433
//*       TBLOOK    exec        Examine and update any table        *   FILE 433
//*                                                                 *   FILE 433
//*       TEXAMU    exec        TBLOOK from the memberlist          *   FILE 433
//*                                                                 *   FILE 433
//*       TRAPOUT   exec        Trap trace output to DASD           *   FILE 433
//*                                                                 *   FILE 433
//*       UPDSTAT   exec        Update ISPF statistics              *   FILE 433
//*                                                                 *   FILE 433
//*       VCX       exec        Show IDCAMS for any file            *   FILE 433
//*                                                                 *   FILE 433
//*       VWBR      exec        View from Browse                    *   FILE 433
//*                                                                 *   FILE 433
//*       WB        exec        Insert "Written by" data            *   FILE 433
//*                                                                 *   FILE 433
//*       WBNAME    fragment    Data for WB                         *   FILE 433
//*                                                                 *   FILE 433
```

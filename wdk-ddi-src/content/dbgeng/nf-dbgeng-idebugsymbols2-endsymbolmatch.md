---
UID: NF:dbgeng.IDebugSymbols2.EndSymbolMatch
title: IDebugSymbols2::EndSymbolMatch (dbgeng.h)
description: The EndSymbolMatch method releases the resources used by a symbol search. This method belongs to the IDebugSymbols2 interface.
old-location: debugger\endsymbolmatch.htm
tech.root: debugger
ms.date: 05/03/2018
keywords: ["IDebugSymbols2::EndSymbolMatch"]
ms.keywords: EndSymbolMatch, EndSymbolMatch method [Windows Debugging], EndSymbolMatch method [Windows Debugging],IDebugSymbols interface, EndSymbolMatch method [Windows Debugging],IDebugSymbols2 interface, EndSymbolMatch method [Windows Debugging],IDebugSymbols3 interface, IDebugSymbols interface [Windows Debugging],EndSymbolMatch method, IDebugSymbols2 interface [Windows Debugging],EndSymbolMatch method, IDebugSymbols2.EndSymbolMatch, IDebugSymbols2::EndSymbolMatch, IDebugSymbols3 interface [Windows Debugging],EndSymbolMatch method, IDebugSymbols3::EndSymbolMatch, IDebugSymbols::EndSymbolMatch, IDebugSymbols_1661cc8a-ad5c-4cd3-83fe-f829bd07e453.xml, dbgeng/IDebugSymbols2::EndSymbolMatch, dbgeng/IDebugSymbols3::EndSymbolMatch, dbgeng/IDebugSymbols::EndSymbolMatch, debugger.endsymbolmatch
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - IDebugSymbols2::EndSymbolMatch
 - dbgeng/IDebugSymbols2::EndSymbolMatch
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dbgeng.h
api_name:
 - IDebugSymbols2::EndSymbolMatch
---

# IDebugSymbols2::EndSymbolMatch


## -description

The <b>EndSymbolMatch</b> method releases the resources used by a symbol search.

## -parameters

### -param Handle 

[in]
Specifies the handle returned by <a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-startsymbolmatch">StartSymbolMatch</a> when the search was initialized.

## -returns

This method may also return error values.  See <a href="/windows-hardware/drivers/debugger/hresult-values">Return Values</a> for more details.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>

## -remarks

This method releases the resources held by the engine during a symbol search.  After these resources are released, the handle becomes invalid, so it must not be passed to <a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-getnextsymbolmatch">GetNextSymbolMatch</a> after it has been passed to this method.

For more information about symbols, see <a href="/windows-hardware/drivers/debugger/symbols4">Symbols</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-getnextsymbolmatch">GetNextSymbolMatch</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols">IDebugSymbols</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols2">IDebugSymbols2</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols3">IDebugSymbols3</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-startsymbolmatch">StartSymbolMatch</a>


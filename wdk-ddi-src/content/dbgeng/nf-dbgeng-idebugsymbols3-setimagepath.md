---
UID: NF:dbgeng.IDebugSymbols3.SetImagePath
title: IDebugSymbols3::SetImagePath (dbgeng.h)
description: The SetImagePath method sets the executable image path. This method belongs to the IDebugSymbols3 interface.
old-location: debugger\setimagepath.htm
tech.root: debugger
ms.date: 05/03/2018
keywords: ["IDebugSymbols3::SetImagePath"]
ms.keywords: IDebugSymbols interface [Windows Debugging],SetImagePath method, IDebugSymbols2 interface [Windows Debugging],SetImagePath method, IDebugSymbols2::SetImagePath, IDebugSymbols3 interface [Windows Debugging],SetImagePath method, IDebugSymbols3.SetImagePath, IDebugSymbols3::SetImagePath, IDebugSymbols::SetImagePath, IDebugSymbols_062aa9c4-33c9-4a73-a11f-7d5e6b94e96c.xml, SetImagePath, SetImagePath method [Windows Debugging], SetImagePath method [Windows Debugging],IDebugSymbols interface, SetImagePath method [Windows Debugging],IDebugSymbols2 interface, SetImagePath method [Windows Debugging],IDebugSymbols3 interface, dbgeng/IDebugSymbols2::SetImagePath, dbgeng/IDebugSymbols3::SetImagePath, dbgeng/IDebugSymbols::SetImagePath, debugger.setimagepath
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
 - IDebugSymbols3::SetImagePath
 - dbgeng/IDebugSymbols3::SetImagePath
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dbgeng.h
api_name:
 - IDebugSymbols3::SetImagePath
---

# IDebugSymbols3::SetImagePath


## -description

The <b>SetImagePath</b>  method sets the executable image path.

## -parameters

### -param Path 

[in]
Specifies the new executable image path.  This is a string that contains directories separated by semicolons (<b>;</b>).

## -returns

This method can also return error values.  See <a href="/windows-hardware/drivers/debugger/hresult-values">Return Values</a> for more details.

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

The executable image path is used by the engine when searching for executable images.

The executable image path can consist of several directories separated by semicolons.  These directories are searched in order.

## -see-also

<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-appendimagepath">AppendImagePath</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-getimagepath">GetImagePath</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols">IDebugSymbols</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols2">IDebugSymbols2</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols3">IDebugSymbols3</a>


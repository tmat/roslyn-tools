﻿**Sign Tool Data**

This file is used to describe the set of binaries that need to be signed by MicroBuild.  The tool assumes this 
file exists at `build\config\SignToolData.json`.  It can be overridden via the `-configFile` argument.

Here is a sample:

```json
{
    "sign": [
        {
            "certificate": "Microsoft402",
            "strongName": "MsSharedLib72",
            "values": [
                "csc.exe",
                "csccore\\csc.exe",
                "csi.exe",
                "csicore\\csi.exe",
                "InteractiveHost.exe",
                "Microsoft.Build.Tasks.CodeAnalysis.dll",
                "Microsoft.CodeAnalysis.CSharp.dll",
                "Microsoft.CodeAnalysis.CSharp.EditorFeatures.dll",
                "Microsoft.CodeAnalysis.CSharp.Features.dll",
                "Microsoft.CodeAnalysis.CSharp.InteractiveEditorFeatures.dll",
                "Microsoft.CodeAnalysis.CSharp.Scripting.dll",
                "Microsoft.CodeAnalysis.CSharp.Workspaces.dll",
                "Microsoft.CodeAnalysis.dll",
                "Microsoft.CodeAnalysis.EditorFeatures.dll",
                "Microsoft.CodeAnalysis.EditorFeatures.Next.dll",
                "Microsoft.CodeAnalysis.EditorFeatures.Text.dll",
                "Microsoft.CodeAnalysis.Features.dll",
                "Microsoft.CodeAnalysis.InteractiveEditorFeatures.dll",
                "Microsoft.CodeAnalysis.InteractiveFeatures.dll",
                "Microsoft.CodeAnalysis.Remote.ServiceHub.dll",
                "Microsoft.CodeAnalysis.Remote.Workspaces.dll",
                "Microsoft.CodeAnalysis.Scripting.dll",
                "Microsoft.CodeAnalysis.VisualBasic.dll",
                "Microsoft.CodeAnalysis.VisualBasic.EditorFeatures.dll",
                "Microsoft.CodeAnalysis.VisualBasic.Features.dll",
                "Microsoft.CodeAnalysis.VisualBasic.InteractiveEditorFeatures.dll",
                "Microsoft.CodeAnalysis.VisualBasic.Scripting.dll",
                "Microsoft.CodeAnalysis.VisualBasic.Workspaces.dll",
                "Microsoft.CodeAnalysis.Workspaces.Desktop.dll",
                "Microsoft.CodeAnalysis.Workspaces.dll",
                "Microsoft.DiaSymReader.PortablePdb.dll",
                "Microsoft.VisualStudio.CSharp.Repl.dll",
                "Microsoft.VisualStudio.InteractiveServices.dll",
                "Microsoft.VisualStudio.InteractiveWindow.dll",
                "Microsoft.VisualStudio.LanguageServices.CSharp.dll",
                "Microsoft.VisualStudio.LanguageServices.dll",
                "Microsoft.VisualStudio.LanguageServices.Implementation.dll",
                "Microsoft.VisualStudio.LanguageServices.Next.dll",
                "Microsoft.VisualStudio.LanguageServices.SolutionExplorer.dll",
                "Microsoft.VisualStudio.LanguageServices.VisualBasic.dll",
                "Microsoft.VisualStudio.VisualBasic.Repl.dll",
                "Microsoft.VisualStudio.VsInteractiveWindow.dll",
                "Pdb2Xml.exe",
                "Roslyn.Compilers.Extension.dll",
                "Roslyn.Hosting.Diagnostics.dll",
                "Roslyn.VisualStudio.DiagnosticsWindow.dll",
                "Roslyn.VisualStudio.InteractiveComponents.dll",
                "Roslyn.VisualStudio.Setup.Interactive.dll",
                "SDK\\Roslyn.SyntaxVisualizer.DgmlHelper.dll",
                "SDK\\Roslyn.SyntaxVisualizer.Control.dll",
                "SDK\\Roslyn.SyntaxVisualizer.Extension.dll",
                "SDK\\Roslyn.Templates.dll",
                "vbc.exe",
                "vbccore\\vbc.exe",
                "VBCSCompiler.exe",
                "vbi.exe",
                "vbicore\\vbi.exe"
              ]
        },
        {
            "certificate": "WindowsPhone623",
            "strongName": "MsSharedLib72",
            "values": [
                "Microsoft.CodeAnalysis.ExpressionEvaluator.ExpressionCompiler.dll",
                "Microsoft.CodeAnalysis.ExpressionEvaluator.ResultProvider.dll",
                "Microsoft.CodeAnalysis.CSharp.ExpressionEvaluator.ExpressionCompiler.dll",
                "Microsoft.CodeAnalysis.CSharp.ExpressionEvaluator.ResultProvider.dll",
                "Microsoft.CodeAnalysis.VisualBasic.ExpressionEvaluator.ExpressionCompiler.dll",
                "Microsoft.CodeAnalysis.VisualBasic.ExpressionEvaluator.ResultProvider.dll"
            ]
        },
        {
            "certificate": "MicrosoftSHA1Win8WinBlue",
            "strongName": "MsSharedLib72",
            "values": [
                "NetFX20\\Microsoft.CodeAnalysis.ExpressionEvaluator.ResultProvider.dll",
                "NetFX20\\Microsoft.CodeAnalysis.CSharp.ExpressionEvaluator.ResultProvider.dll",
                "NetFX20\\Microsoft.CodeAnalysis.VisualBasic.ExpressionEvaluator.ResultProvider.dll"
            ]
        },
        {
            "certificate": "VsixSHA2",
            "strongName": null,
            "values": [
                "ExpressionEvaluatorPackage.vsix",
                "Microsoft.VisualStudio.VsInteractiveWindow.vsix",
                "Roslyn.Compilers.Extension.vsix",
                "Roslyn.Deployment.Full.vsix",
                "Roslyn.Deployment.Full.Next.vsix",
                "Roslyn.VisualStudio.DiagnosticsWindow.vsix",
                "Roslyn.VisualStudio.InteractiveComponents.vsix",
                "Roslyn.VisualStudio.Setup.Interactive.vsix",
                "Roslyn.VisualStudio.Setup.Next.vsix",
                "Roslyn.VisualStudio.Setup.vsix",
                "RoslynDeployment.vsix",
                "SDK\\Roslyn Templates\\Release\\Roslyn SDK.vsix"
            ]
        }
    ],

    // Binaries which are included in VSIX above which are not to be signed.
    "exclude": [
        "Esent.Interop.dll",
        "Microsoft.CodeAnalysis.Elfie.dll",
        "Microsoft.DiaSymReader.dll",
        "Microsoft.DiaSymReader.Native.amd64.dll",
        "Microsoft.DiaSymReader.Native.x86.dll",
        "Newtonsoft.Json.dll",
        "StreamJsonRpc.dll",
        "StreamJsonRpc.resources.dll",
        "System.Reflection.Metadata.dll",
        "System.Collections.Immutable.dll",
        "System.Diagnostics.StackTrace.dll",
        "System.IO.FileSystem.dll",
        "System.IO.FileSystem.Primitives.dll",
        "System.Composition.AttributedModel.dll",
        "System.Composition.Convention.dll",
        "System.Composition.Hosting.dll",
        "System.Composition.TypedParts.dll",
        "System.Composition.Runtime.dll",
        "Microsoft.Build.Conversion.Core.dll",
        "Microsoft.Build.dll",
        "Microsoft.Build.Engine.dll",
        "Microsoft.Build.Framework.dll",
        "Microsoft.Build.Tasks.Core.dll",
        "Microsoft.Build.Utilities.Core.dll",
        "Microsoft.VisualStudio.Threading.dll",
        "Microsoft.VisualStudio.Validation.dll"
    ]
}
```
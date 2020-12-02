
---
title: "GetEncryptionScope"
title_tag: "Function GetEncryptionScope | Module storage | Package Azure"
meta_desc: "Explore the GetEncryptionScope function of the storage module, including examples, input properties, output properties, and supporting types. Use this data source to access information about an existing Storage Encryption Scope."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

Use this data source to access information about an existing Storage Encryption Scope.


{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}

{{% example csharp %}}
```csharp
using Pulumi;
using Azure = Pulumi.Azure;

class MyStack : Stack
{
    public MyStack()
    {
        var exampleAccount = Output.Create(Azure.Storage.GetAccount.InvokeAsync(new Azure.Storage.GetAccountArgs
        {
            Name = "storageaccountname",
            ResourceGroupName = "resourcegroupname",
        }));
        var exampleEncryptionScope = exampleAccount.Apply(exampleAccount => Output.Create(Azure.Storage.GetEncryptionScope.InvokeAsync(new Azure.Storage.GetEncryptionScopeArgs
        {
            Name = "existingStorageES",
            StorageAccountId = exampleAccount.Id,
        })));
        this.Id = exampleEncryptionScope.Apply(exampleEncryptionScope => exampleEncryptionScope.Id);
    }

    [Output("id")]
    public Output<string> Id { get; set; }
}
```

{{% /example %}}

{{% example go %}}
```go
package main

import (
	"github.com/pulumi/pulumi-azure/sdk/v3/go/azure/storage"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		opt0 := "resourcegroupname"
		exampleAccount, err := storage.LookupAccount(ctx, &storage.LookupAccountArgs{
			Name:              "storageaccountname",
			ResourceGroupName: &opt0,
		}, nil)
		if err != nil {
			return err
		}
		exampleEncryptionScope, err := storage.LookupEncryptionScope(ctx, &storage.LookupEncryptionScopeArgs{
			Name:             "existingStorageES",
			StorageAccountId: exampleAccount.Id,
		}, nil)
		if err != nil {
			return err
		}
		ctx.Export("id", exampleEncryptionScope.Id)
		return nil
	})
}
```

{{% /example %}}

{{% example python %}}
```python
import pulumi
import pulumi_azure as azure

example_account = azure.storage.get_account(name="storageaccountname",
    resource_group_name="resourcegroupname")
example_encryption_scope = azure.storage.get_encryption_scope(name="existingStorageES",
    storage_account_id=example_account.id)
pulumi.export("id", example_encryption_scope.id)
```

{{% /example %}}

{{% example typescript %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as azure from "@pulumi/azure";

const exampleAccount = azure.storage.getAccount({
    name: "storageaccountname",
    resourceGroupName: "resourcegroupname",
});
const exampleEncryptionScope = exampleAccount.then(exampleAccount => azure.storage.getEncryptionScope({
    name: "existingStorageES",
    storageAccountId: exampleAccount.id,
}));
export const id = exampleEncryptionScope.then(exampleEncryptionScope => exampleEncryptionScope.id);
```

{{% /example %}}

{{% /examples %}}


## Using GetEncryptionScope {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getEncryptionScope<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/storage/#GetEncryptionScopeArgs">GetEncryptionScopeArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/azure/storage/#GetEncryptionScopeResult">GetEncryptionScopeResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_encryption_scope(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">storage_account_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetEncryptionScopeResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>LookupEncryptionScope<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/v3/go/azure/storage?tab=doc#LookupEncryptionScopeArgs">LookupEncryptionScopeArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-azure/sdk/v3/go/azure/storage?tab=doc#LookupEncryptionScopeResult">LookupEncryptionScopeResult</a></span>, error)</span></code></pre></div>

> Note: This function is named `LookupEncryptionScope` in the Go SDK.

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetEncryptionScope </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Storage.GetEncryptionScopeResult.html">GetEncryptionScopeResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Azure/Pulumi.Azure.Storage.GetEncryptionScopeArgs.html">GetEncryptionScopeArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The name of this Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="storageaccountid_csharp">
<a href="#storageaccountid_csharp" style="color: inherit; text-decoration: inherit;">Storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Storage Account where this Storage Encryption Scope exists.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The name of this Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="storageaccountid_go">
<a href="#storageaccountid_go" style="color: inherit; text-decoration: inherit;">Storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Storage Account where this Storage Encryption Scope exists.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The name of this Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="storageaccountid_nodejs">
<a href="#storageaccountid_nodejs" style="color: inherit; text-decoration: inherit;">storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Storage Account where this Storage Encryption Scope exists.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The name of this Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="storage_account_id_python">
<a href="#storage_account_id_python" style="color: inherit; text-decoration: inherit;">storage_<wbr>account_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Storage Account where this Storage Encryption Scope exists.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetEncryptionScope Result {#result}

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyvaultkeyid_csharp">
<a href="#keyvaultkeyid_csharp" style="color: inherit; text-decoration: inherit;">Key<wbr>Vault<wbr>Key<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Key Vault Key.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="name_csharp">
<a href="#name_csharp" style="color: inherit; text-decoration: inherit;">Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="source_csharp">
<a href="#source_csharp" style="color: inherit; text-decoration: inherit;">Source</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The source of the Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="storageaccountid_csharp">
<a href="#storageaccountid_csharp" style="color: inherit; text-decoration: inherit;">Storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyvaultkeyid_go">
<a href="#keyvaultkeyid_go" style="color: inherit; text-decoration: inherit;">Key<wbr>Vault<wbr>Key<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Key Vault Key.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="name_go">
<a href="#name_go" style="color: inherit; text-decoration: inherit;">Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="source_go">
<a href="#source_go" style="color: inherit; text-decoration: inherit;">Source</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The source of the Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="storageaccountid_go">
<a href="#storageaccountid_go" style="color: inherit; text-decoration: inherit;">Storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyvaultkeyid_nodejs">
<a href="#keyvaultkeyid_nodejs" style="color: inherit; text-decoration: inherit;">key<wbr>Vault<wbr>Key<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Key Vault Key.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="name_nodejs">
<a href="#name_nodejs" style="color: inherit; text-decoration: inherit;">name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="source_nodejs">
<a href="#source_nodejs" style="color: inherit; text-decoration: inherit;">source</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The source of the Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="storageaccountid_nodejs">
<a href="#storageaccountid_nodejs" style="color: inherit; text-decoration: inherit;">storage<wbr>Account<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="key_vault_key_id_python">
<a href="#key_vault_key_id_python" style="color: inherit; text-decoration: inherit;">key_<wbr>vault_<wbr>key_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The ID of the Key Vault Key.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="name_python">
<a href="#name_python" style="color: inherit; text-decoration: inherit;">name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="source_python">
<a href="#source_python" style="color: inherit; text-decoration: inherit;">source</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The source of the Storage Encryption Scope.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="storage_account_id_python">
<a href="#storage_account_id_python" style="color: inherit; text-decoration: inherit;">storage_<wbr>account_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-azure">https://github.com/pulumi/pulumi-azure</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`azurerm` Terraform Provider](https://github.com/terraform-providers/terraform-provider-azurerm).</dd>
</dl>

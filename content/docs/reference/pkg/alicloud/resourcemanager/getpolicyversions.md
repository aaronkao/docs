
---
title: "GetPolicyVersions"
title_tag: "Function GetPolicyVersions | Module resourcemanager | Package AliCloud"
meta_desc: "Explore the GetPolicyVersions function of the resourcemanager module, including examples, input properties, output properties, and supporting types. This data source provides the Resource Manager Policy Versions of the current Alibaba Cloud user."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

This data source provides the Resource Manager Policy Versions of the current Alibaba Cloud user.

> **NOTE:**  Available in 1.85.0+.



{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}

{{% example csharp %}}
```csharp
using Pulumi;
using AliCloud = Pulumi.AliCloud;

class MyStack : Stack
{
    public MyStack()
    {
        var @default = Output.Create(AliCloud.ResourceManager.GetPolicyVersions.InvokeAsync(new AliCloud.ResourceManager.GetPolicyVersionsArgs
        {
            PolicyName = "tftest",
            PolicyType = "Custom",
        }));
        this.FirstPolicyVersionId = @default.Apply(@default => @default.Versions[0].Id);
    }

    [Output("firstPolicyVersionId")]
    public Output<string> FirstPolicyVersionId { get; set; }
}
```
{{% /example %}}

{{% example go %}}
Coming soon!
{{% /example %}}

{{% example python %}}
```python
import pulumi
import pulumi_alicloud as alicloud

default = alicloud.resourcemanager.get_policy_versions(policy_name="tftest",
    policy_type="Custom")
pulumi.export("firstPolicyVersionId", default.versions[0]["id"])
```
{{% /example %}}

{{% example typescript %}}
```typescript
import * as pulumi from "@pulumi/pulumi";
import * as alicloud from "@pulumi/alicloud";

const defaultPolicyVersions = pulumi.output(alicloud.resourcemanager.getPolicyVersions({
    policyName: "tftest",
    policyType: "Custom",
}, { async: true }));

export const firstPolicyVersionId = defaultPolicyVersions.versions[0].id;
```
{{% /example %}}

{{% /examples %}}


## Using GetPolicyVersions {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getPolicyVersions<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/resourcemanager/#GetPolicyVersionsArgs">GetPolicyVersionsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/resourcemanager/#GetPolicyVersionsResult">GetPolicyVersionsResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">function </span> get_policy_versions(</span>ids=None<span class="p">, </span>output_file=None<span class="p">, </span>policy_name=None<span class="p">, </span>policy_type=None<span class="p">, </span>opts=None<span class="p">)</span></code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetPolicyVersions<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/resourcemanager?tab=doc#GetPolicyVersionsArgs">GetPolicyVersionsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/resourcemanager?tab=doc#GetPolicyVersionsResult">GetPolicyVersionsResult</a></span>, error)</span></code></pre></div>

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetPolicyVersions </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.Resourcemanager.GetPolicyVersionsResult.html">GetPolicyVersionsResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.ResourceManager.GetPolicyVersionsArgs.html">GetPolicyVersionsArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="policyname_csharp">
<a href="#policyname_csharp" style="color: inherit; text-decoration: inherit;">Policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The name of the policy.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="policytype_csharp">
<a href="#policytype_csharp" style="color: inherit; text-decoration: inherit;">Policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The type of the policy. Valid values:`Custom` and `System`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_csharp">
<a href="#ids_csharp" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">List&lt;string&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_csharp">
<a href="#outputfile_csharp" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="policyname_go">
<a href="#policyname_go" style="color: inherit; text-decoration: inherit;">Policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The name of the policy.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="policytype_go">
<a href="#policytype_go" style="color: inherit; text-decoration: inherit;">Policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The type of the policy. Valid values:`Custom` and `System`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_go">
<a href="#ids_go" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">[]string</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_go">
<a href="#outputfile_go" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="policyname_nodejs">
<a href="#policyname_nodejs" style="color: inherit; text-decoration: inherit;">policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The name of the policy.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="policytype_nodejs">
<a href="#policytype_nodejs" style="color: inherit; text-decoration: inherit;">policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The type of the policy. Valid values:`Custom` and `System`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_nodejs">
<a href="#ids_nodejs" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string[]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_nodejs">
<a href="#outputfile_nodejs" style="color: inherit; text-decoration: inherit;">output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="policy_name_python">
<a href="#policy_name_python" style="color: inherit; text-decoration: inherit;">policy_<wbr>name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The name of the policy.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="policy_type_python">
<a href="#policy_type_python" style="color: inherit; text-decoration: inherit;">policy_<wbr>type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The type of the policy. Valid values:`Custom` and `System`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_python">
<a href="#ids_python" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">List[str]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="output_file_python">
<a href="#output_file_python" style="color: inherit; text-decoration: inherit;">output_<wbr>file</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetPolicyVersions Result {#result}

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
        <span id="ids_csharp">
<a href="#ids_csharp" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">List&lt;string&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policyname_csharp">
<a href="#policyname_csharp" style="color: inherit; text-decoration: inherit;">Policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policytype_csharp">
<a href="#policytype_csharp" style="color: inherit; text-decoration: inherit;">Policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="versions_csharp">
<a href="#versions_csharp" style="color: inherit; text-decoration: inherit;">Versions</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getpolicyversionsversion">List&lt;Pulumi.<wbr>Ali<wbr>Cloud.<wbr>Resource<wbr>Manager.<wbr>Outputs.<wbr>Get<wbr>Policy<wbr>Versions<wbr>Version&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of policy versions. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_csharp">
<a href="#outputfile_csharp" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
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
        <span id="ids_go">
<a href="#ids_go" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">[]string</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policyname_go">
<a href="#policyname_go" style="color: inherit; text-decoration: inherit;">Policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policytype_go">
<a href="#policytype_go" style="color: inherit; text-decoration: inherit;">Policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="versions_go">
<a href="#versions_go" style="color: inherit; text-decoration: inherit;">Versions</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getpolicyversionsversion">[]Get<wbr>Policy<wbr>Versions<wbr>Version</a></span>
    </dt>
    <dd>{{% md %}}A list of policy versions. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_go">
<a href="#outputfile_go" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
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
        <span id="ids_nodejs">
<a href="#ids_nodejs" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string[]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policyname_nodejs">
<a href="#policyname_nodejs" style="color: inherit; text-decoration: inherit;">policy<wbr>Name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policytype_nodejs">
<a href="#policytype_nodejs" style="color: inherit; text-decoration: inherit;">policy<wbr>Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="versions_nodejs">
<a href="#versions_nodejs" style="color: inherit; text-decoration: inherit;">versions</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getpolicyversionsversion">Get<wbr>Policy<wbr>Versions<wbr>Version[]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy versions. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_nodejs">
<a href="#outputfile_nodejs" style="color: inherit; text-decoration: inherit;">output<wbr>File</a>
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
        <span id="ids_python">
<a href="#ids_python" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">List[str]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy version IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policy_name_python">
<a href="#policy_name_python" style="color: inherit; text-decoration: inherit;">policy_<wbr>name</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="policy_type_python">
<a href="#policy_type_python" style="color: inherit; text-decoration: inherit;">policy_<wbr>type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="versions_python">
<a href="#versions_python" style="color: inherit; text-decoration: inherit;">versions</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getpolicyversionsversion">List[Get<wbr>Policy<wbr>Versions<wbr>Version]</a></span>
    </dt>
    <dd>{{% md %}}A list of policy versions. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="output_file_python">
<a href="#output_file_python" style="color: inherit; text-decoration: inherit;">output_<wbr>file</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Supporting Types


<h4 id="getpolicyversionsversion">Get<wbr>Policy<wbr>Versions<wbr>Version</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/alicloud/types/output/#GetPolicyVersionsVersion">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/resourcemanager?tab=doc#GetPolicyVersionsVersion">output</a> API doc for this type.
{{% /choosable %}}
{{% choosable language csharp %}}
> See the   <a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.ResourceManager.Outputs.GetPolicyVersionsVersion.html">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="createdate_csharp">
<a href="#createdate_csharp" style="color: inherit; text-decoration: inherit;">Create<wbr>Date</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the resource, the value is `<policy_name>`:`<version_id>`.
* `version_id`- The ID of the policy version.
* `create_date`- The time when the policy version was created.
* `is_default_version`- Indicates whether the policy version is the default version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="isdefaultversion_csharp">
<a href="#isdefaultversion_csharp" style="color: inherit; text-decoration: inherit;">Is<wbr>Default<wbr>Version</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">bool</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="versionid_csharp">
<a href="#versionid_csharp" style="color: inherit; text-decoration: inherit;">Version<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="createdate_go">
<a href="#createdate_go" style="color: inherit; text-decoration: inherit;">Create<wbr>Date</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the resource, the value is `<policy_name>`:`<version_id>`.
* `version_id`- The ID of the policy version.
* `create_date`- The time when the policy version was created.
* `is_default_version`- Indicates whether the policy version is the default version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="isdefaultversion_go">
<a href="#isdefaultversion_go" style="color: inherit; text-decoration: inherit;">Is<wbr>Default<wbr>Version</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#boolean">bool</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="versionid_go">
<a href="#versionid_go" style="color: inherit; text-decoration: inherit;">Version<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="createdate_nodejs">
<a href="#createdate_nodejs" style="color: inherit; text-decoration: inherit;">create<wbr>Date</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The ID of the resource, the value is `<policy_name>`:`<version_id>`.
* `version_id`- The ID of the policy version.
* `create_date`- The time when the policy version was created.
* `is_default_version`- Indicates whether the policy version is the default version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="isdefaultversion_nodejs">
<a href="#isdefaultversion_nodejs" style="color: inherit; text-decoration: inherit;">is<wbr>Default<wbr>Version</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/boolean">boolean</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="versionid_nodejs">
<a href="#versionid_nodejs" style="color: inherit; text-decoration: inherit;">version<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="create_date_python">
<a href="#create_date_python" style="color: inherit; text-decoration: inherit;">create_<wbr>date</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The ID of the resource, the value is `<policy_name>`:`<version_id>`.
* `version_id`- The ID of the policy version.
* `create_date`- The time when the policy version was created.
* `is_default_version`- Indicates whether the policy version is the default version.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="is_default_version_python">
<a href="#is_default_version_python" style="color: inherit; text-decoration: inherit;">is_<wbr>default_<wbr>version</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">bool</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="version_id_python">
<a href="#version_id_python" style="color: inherit; text-decoration: inherit;">version_<wbr>id</a>
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
	<dd><a href="https://github.com/pulumi/pulumi-alicloud">https://github.com/pulumi/pulumi-alicloud</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`alicloud` Terraform Provider](https://github.com/terraform-providers/terraform-provider-alicloud).</dd>
</dl>

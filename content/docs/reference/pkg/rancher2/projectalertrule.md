
---
title: "ProjectAlertRule"
block_external_search_index: true
---






## Create a ProjectAlertRule Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ProjectAlertRule">ProjectAlertRule</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ProjectAlertRuleArgs">ProjectAlertRuleArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">ProjectAlertRule</span><span class="p">(resource_name, opts=None, </span>annotations=None<span class="p">, </span>group_id=None<span class="p">, </span>group_interval_seconds=None<span class="p">, </span>group_wait_seconds=None<span class="p">, </span>inherited=None<span class="p">, </span>labels=None<span class="p">, </span>metric_rule=None<span class="p">, </span>name=None<span class="p">, </span>pod_rule=None<span class="p">, </span>project_id=None<span class="p">, </span>repeat_interval_seconds=None<span class="p">, </span>severity=None<span class="p">, </span>workload_rule=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewProjectAlertRule<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleArgs">ProjectAlertRuleArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRule">ProjectAlertRule</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ProjectAlertRule.html">ProjectAlertRule</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2.ProjectAlertRuleArgs.html">ProjectAlertRuleArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">*Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">*Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">*Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pod_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>project_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## ProjectAlertRule Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object></span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">*Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">*Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">*Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>pod_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>project_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>workload_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing ProjectAlertRule Resource

Get an existing ProjectAlertRule resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ProjectAlertRuleState">ProjectAlertRuleState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/rancher2/#ProjectAlertRule">ProjectAlertRule</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>annotations=None<span class="p">, </span>group_id=None<span class="p">, </span>group_interval_seconds=None<span class="p">, </span>group_wait_seconds=None<span class="p">, </span>inherited=None<span class="p">, </span>labels=None<span class="p">, </span>metric_rule=None<span class="p">, </span>name=None<span class="p">, </span>pod_rule=None<span class="p">, </span>project_id=None<span class="p">, </span>repeat_interval_seconds=None<span class="p">, </span>severity=None<span class="p">, </span>workload_rule=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetProjectAlertRule<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleState">ProjectAlertRuleState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRule">ProjectAlertRule</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ProjectAlertRule.html">ProjectAlertRule</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Rancher2/Pulumi.Rancher2..ProjectAlertRuleState.html">ProjectAlertRuleState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">*Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">*Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">*Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group<wbr>Wait<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pod<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload<wbr>Rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule?</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>annotations</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule annotations (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule alert group ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group interval seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>group_<wbr>wait_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule group wait seconds. Default: `180` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>inherited</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}The project alert rule inherited. Default: `true` (bool)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}The project alert rule labels (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>metric_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulemetricrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule metric rule. ConflictsWith: `"pod_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule name (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>pod_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertrulepodrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule pod rule. ConflictsWith: `"metric_rule", "workload_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project id where create project alert rule (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>repeat_<wbr>interval_<wbr>seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}The project alert rule wait seconds. Default: `3600` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>severity</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The project alert rule severity. Supported values : `"critical" | "info" | "warning"`. Default: `critical` (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload_<wbr>rule</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#projectalertruleworkloadrule">Dict[Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule]</a></span>
    </dt>
    <dd>{{% md %}}The project alert rule workload rule. ConflictsWith: `"metric_rule", "pod_rule"`` (list Maxitems:1)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Project<wbr>Alert<wbr>Rule<wbr>Metric<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ProjectAlertRuleMetricRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ProjectAlertRuleMetricRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleMetricRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleMetricRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">double</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">float64</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>comparison</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule comparison. Supported values : `"equal" | "greater-or-equal" | "greater-than" | "less-or-equal" | "less-than" | "not-equal" | "has-value"`. Default: `equal`  (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule description (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>duration</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule duration (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Metric rule expression (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>threshold<wbr>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Metric rule threshold value (float64)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Project<wbr>Alert<wbr>Rule<wbr>Pod<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ProjectAlertRulePodRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ProjectAlertRulePodRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRulePodRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRulePodRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Pod rule condition. Supported values : `"notrunning" | "notscheduled" | "restarts"`. Default: `notrunning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Pod<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Pod ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Restart<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Pod rule restart interval seconds. Default: `300` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Restart<wbr>Times</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Pod rule restart times. Default: `3`  (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Pod rule condition. Supported values : `"notrunning" | "notscheduled" | "restarts"`. Default: `notrunning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Pod<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Pod ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Restart<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Pod rule restart interval seconds. Default: `300` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Restart<wbr>Times</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Pod rule restart times. Default: `3`  (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Pod rule condition. Supported values : `"notrunning" | "notscheduled" | "restarts"`. Default: `notrunning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>pod<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Pod ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>restart<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Pod rule restart interval seconds. Default: `300` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>restart<wbr>Times</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Pod rule restart times. Default: `3`  (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>condition</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Pod rule condition. Supported values : `"notrunning" | "notscheduled" | "restarts"`. Default: `notrunning` (string)
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>pod<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Pod ID (string)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>restart<wbr>Interval<wbr>Seconds</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Pod rule restart interval seconds. Default: `300` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>restart<wbr>Times</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Pod rule restart times. Default: `3`  (int)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Project<wbr>Alert<wbr>Rule<wbr>Workload<wbr>Rule</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/input/#ProjectAlertRuleWorkloadRule">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/rancher2/types/output/#ProjectAlertRuleWorkloadRule">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleWorkloadRuleArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-rancher2/sdk/go/rancher2/?tab=doc#ProjectAlertRuleWorkloadRuleOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Available<wbr>Percentage</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Workload rule available percentage. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dictionary<string, object>?</span>
    </dt>
    <dd>{{% md %}}Workload rule selector (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Workload ID (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Available<wbr>Percentage</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Workload rule available percentage. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">map[string]interface{}</span>
    </dt>
    <dd>{{% md %}}Workload rule selector (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Workload<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Workload ID (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>available<wbr>Percentage</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Workload rule available percentage. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">{[key: string]: any}?</span>
    </dt>
    <dd>{{% md %}}Workload rule selector (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Workload ID (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>available<wbr>Percentage</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Workload rule available percentage. Default: `70` (int)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>selector</span>
        <span class="property-indicator"></span>
        <span class="property-type">Dict[str, Any]</span>
    </dt>
    <dd>{{% md %}}Workload rule selector (map)
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>workload<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Workload ID (string)
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-rancher2">https://github.com/pulumi/pulumi-rancher2</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>

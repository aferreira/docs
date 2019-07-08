---
title: Module aws
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

<a href="../">@pulumi/datadog</a> &gt; aws

<div class="toggleVisible">
<div class="collapsed">
<h2 class="pdoc-module-header toggleButton" title="Click to show Index">Index ▹</h2>
</div>
<div class="expanded">
<h2 class="pdoc-module-header toggleButton" title="Click to hide Index">Index ▾</h2>
<div class="pdoc-module-contents">
<ul>
<li><a href="#Integration">class Integration</a></li>
<li><a href="#IntegrationArgs">interface IntegrationArgs</a></li>
<li><a href="#IntegrationState">interface IntegrationState</a></li>
</ul>

<a href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts">aws/integration.ts</a> 
</div>
</div>
</div>


<h2 class="pdoc-module-header" id="Integration">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L34">class <b>Integration</b></a>
</h2>
<div class="pdoc-module-contents">
<pre class="highlight"><span class='kd'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></pre>
{{% md %}}

Provides a Datadog - Amazon Web Services integration resource. This can be used to create and manage Datadog - Amazon Web Services integration.

Update operations are currently not supported with datadog API so any change forces a new resource.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as datadog from "@pulumi/datadog";

// Create a new Datadog - Amazon Web Services integration
const sandbox = new datadog.aws.Integration("sandbox", {
    accountId: "1234567890",
    accountSpecificNamespaceRules: {
        auto_scaling: false,
        opsworks: false,
    },
    filterTags: ["key:value"],
    hostTags: [
        "key:value",
        "key2:value2",
    ],
    roleName: "DatadogAWSIntegrationRole",
});
```

{{% /md %}}
<h3 class="pdoc-member-header" id="Integration-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L84"> <b>constructor</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span><span class='kd'>new</span> Integration(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#IntegrationArgs'>IntegrationArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</pre>


Create a Integration resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L43">method <b>get</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#IntegrationState'>IntegrationState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Integration'>Integration</a></pre>


Get an existing Integration resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L19">method <b>getProvider</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): ProviderResource | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></pre>

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L54">method <b>isInstance</b></a>
</h3>
<div class="pdoc-member-contents">
{{% md %}}

<pre class="highlight"><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span></pre>


Returns true if the given object is an instance of Integration.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-accountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L64">property <b>accountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>accountId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your AWS Account ID without dashes.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-accountSpecificNamespaceRules">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L68">property <b>accountSpecificNamespaceRules</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>accountSpecificNamespaceRules: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>} | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://api.datadoghq.com/api/v1/integration/aws/available_namespace_rules).

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-externalId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L72">property <b>externalId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>externalId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

AWS External ID

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-filterTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L76">property <b>filterTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>filterTags: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[] | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

Array of EC2 tags (in the form `key:value`) defines a filter that Datadog use when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-hostTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L80">property <b>hostTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>hostTags: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>[] | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</pre>
{{% md %}}

Array of tags (in the form key:value) to add to all hosts and metrics reporting through this integration.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L187">property <b>id</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</pre>
{{% md %}}

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-roleName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L84">property <b>roleName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'>public </span>roleName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your Datadog role delegation name.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="Integration-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L17">property <b>urn</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</pre>
{{% md %}}

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="IntegrationArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L156">interface <b>IntegrationArgs</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

The set of arguments for constructing a Integration resource.

{{% /md %}}
<h3 class="pdoc-member-header" id="IntegrationArgs-accountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L160">property <b>accountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>accountId: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your AWS Account ID without dashes.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationArgs-accountSpecificNamespaceRules">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L164">property <b>accountSpecificNamespaceRules</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>accountSpecificNamespaceRules?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;}&gt;;</pre>
{{% md %}}

Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://api.datadoghq.com/api/v1/integration/aws/available_namespace_rules).

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationArgs-filterTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L168">property <b>filterTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>filterTags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}

Array of EC2 tags (in the form `key:value`) defines a filter that Datadog use when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationArgs-hostTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L172">property <b>hostTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>hostTags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}

Array of tags (in the form key:value) to add to all hosts and metrics reporting through this integration.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationArgs-roleName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L176">property <b>roleName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>roleName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your Datadog role delegation name.

{{% /md %}}
</div>
</div>
<h2 class="pdoc-module-header" id="IntegrationState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L126">interface <b>IntegrationState</b></a>
</h2>
<div class="pdoc-module-contents">
{{% md %}}

Input properties used for looking up and filtering Integration resources.

{{% /md %}}
<h3 class="pdoc-member-header" id="IntegrationState-accountId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L130">property <b>accountId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>accountId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your AWS Account ID without dashes.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationState-accountSpecificNamespaceRules">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L134">property <b>accountSpecificNamespaceRules</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>accountSpecificNamespaceRules?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;{[key: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>]: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;}&gt;;</pre>
{{% md %}}

Enables or disables metric collection for specific AWS namespaces for this AWS account only. A list of namespaces can be found at the [available namespace rules API endpoint](https://api.datadoghq.com/api/v1/integration/aws/available_namespace_rules).

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationState-externalId">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L138">property <b>externalId</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>externalId?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

AWS External ID

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationState-filterTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L142">property <b>filterTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>filterTags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}

Array of EC2 tags (in the form `key:value`) defines a filter that Datadog use when collecting metrics from EC2. Wildcards, such as `?` (for single characters) and `*` (for multiple characters) can also be used.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationState-hostTags">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L146">property <b>hostTags</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>hostTags?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</pre>
{{% md %}}

Array of tags (in the form key:value) to add to all hosts and metrics reporting through this integration.

{{% /md %}}
</div>
<h3 class="pdoc-member-header" id="IntegrationState-roleName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-datadog/blob/101d42e6cc66710053b55a7b8a178b1ef3458a8f/sdk/nodejs/aws/integration.ts#L150">property <b>roleName</b></a>
</h3>
<div class="pdoc-member-contents">
<pre class="highlight"><span class='kd'></span>roleName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</pre>
{{% md %}}

Your Datadog role delegation name.

{{% /md %}}
</div>
</div>
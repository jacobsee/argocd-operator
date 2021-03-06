# API Documentaion

<p>Packages:</p>
<ul>
<li>
<a href="#argoproj.io%2fv1alpha1">argoproj.io/v1alpha1</a>
</li>
</ul>
<h2 id="argoproj.io/v1alpha1">argoproj.io/v1alpha1</h2>
<p>
<p>Package v1alpha1 contains API Schema definitions for the argoproj v1alpha1 API group</p>
</p>
Resource Types:
<ul></ul>
<h3 id="argoproj.io/v1alpha1.ArgoCD">ArgoCD
</h3>
<p>
<p>ArgoCD is the Schema for the argocds API</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>metadata</code></br>
<em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#objectmeta-v1-meta">
Kubernetes meta/v1.ObjectMeta
</a>
</em>
</td>
<td>
Refer to the Kubernetes API documentation for the fields of the
<code>metadata</code> field.
</td>
</tr>
<tr>
<td>
<code>spec</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">
ArgoCDSpec
</a>
</em>
</td>
<td>
<br/>
<br/>
<table>
<tr>
<td>
<code>applicationInstanceLabelKey</code></br>
<em>
string
</em>
</td>
<td>
<p>ApplicationInstanceLabelKey</p>
</td>
</tr>
<tr>
<td>
<code>configManagementPlugins</code></br>
<em>
string
</em>
</td>
<td>
<p>ConfigManagementPlugins is used to specify additional config management plugins.</p>
</td>
</tr>
<tr>
<td>
<code>controller</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDApplicationControllerSpec">
ArgoCDApplicationControllerSpec
</a>
</em>
</td>
<td>
<p>Controller defines the Application Controller options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>dex</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDDexSpec">
ArgoCDDexSpec
</a>
</em>
</td>
<td>
<p>Dex defines the Dex server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>gaTrackingID</code></br>
<em>
string
</em>
</td>
<td>
<p>GATrackingID is the google analytics tracking ID to use.</p>
</td>
</tr>
<tr>
<td>
<code>gaAnonymizeUsers</code></br>
<em>
bool
</em>
</td>
<td>
<p>GAAnonymizeUsers toggles user IDs being hashed before sending to google analytics.</p>
</td>
</tr>
<tr>
<td>
<code>grafana</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDGrafanaSpec">
ArgoCDGrafanaSpec
</a>
</em>
</td>
<td>
<p>Grafana defines the Grafana server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>helpChatURL</code></br>
<em>
string
</em>
</td>
<td>
<p>HelpChatURL is the URL for getting chat help, this will typically be your Slack channel for support.</p>
</td>
</tr>
<tr>
<td>
<code>helpChatText</code></br>
<em>
string
</em>
</td>
<td>
<p>HelpChatText is the text for getting chat help, defaults to &ldquo;Chat now!&rdquo;</p>
</td>
</tr>
<tr>
<td>
<code>image</code></br>
<em>
string
</em>
</td>
<td>
<p>Image is the ArgoCD container image for all ArgoCD components.</p>
</td>
</tr>
<tr>
<td>
<code>import</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDImportSpec">
ArgoCDImportSpec
</a>
</em>
</td>
<td>
<p>Import is the import/restore options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>ingress</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDIngressSpec">
ArgoCDIngressSpec
</a>
</em>
</td>
<td>
<p>Ingress defines the Ingress options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>kustomizeBuildOptions</code></br>
<em>
string
</em>
</td>
<td>
<p>KustomizeBuildOptions is used to specify build options/parameters to use with <code>kustomize build</code>.</p>
</td>
</tr>
<tr>
<td>
<code>oidcConfig</code></br>
<em>
string
</em>
</td>
<td>
<p>OIDCConfig is the configuration as an alternative to dex.</p>
</td>
</tr>
<tr>
<td>
<code>prometheus</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDPrometheusSpec">
ArgoCDPrometheusSpec
</a>
</em>
</td>
<td>
<p>Prometheus defines the Prometheus server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>rbac</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDRBACSpec">
ArgoCDRBACSpec
</a>
</em>
</td>
<td>
<p>RBAC defines the RBAC configuration for Argo CD.</p>
</td>
</tr>
<tr>
<td>
<code>redis</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDRedisSpec">
ArgoCDRedisSpec
</a>
</em>
</td>
<td>
<p>Redis defines the Redis server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>repositories</code></br>
<em>
string
</em>
</td>
<td>
<p>Repositories to configure Argo CD with.</p>
</td>
</tr>
<tr>
<td>
<code>resourceCustomizations</code></br>
<em>
string
</em>
</td>
<td>
<p>ResourceCustomizations customizes resource behavior. Keys are in the form: group/Kind.</p>
</td>
</tr>
<tr>
<td>
<code>resourceExclusions</code></br>
<em>
string
</em>
</td>
<td>
<p>ResourceExclusions is used to completely ignore entire classes of resource group/kinds.</p>
</td>
</tr>
<tr>
<td>
<code>server</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerSpec">
ArgoCDServerSpec
</a>
</em>
</td>
<td>
<p>Server defines the options for the ArgoCD Server component.</p>
</td>
</tr>
<tr>
<td>
<code>sshKnownHosts</code></br>
<em>
string
</em>
</td>
<td>
<p>SSHKnownHosts defines the SSH known hosts data for connecting Git repositories via SSH.</p>
</td>
</tr>
<tr>
<td>
<code>statusBadgeEnabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>StatusBadgeEnabled toggles application status badge feature.</p>
</td>
</tr>
<tr>
<td>
<code>tls</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDTLSSpec">
ArgoCDTLSSpec
</a>
</em>
</td>
<td>
<p>TLS defines the TLS options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>usersAnonymousEnabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>UsersAnonymousEnabled toggles anonymous user access.
The anonymous users get default role permissions specified argocd-rbac-cm.</p>
</td>
</tr>
<tr>
<td>
<code>version</code></br>
<em>
string
</em>
</td>
<td>
<p>Version is the tag to use with the ArgoCD container image for all ArgoCD components.</p>
</td>
</tr>
</table>
</td>
</tr>
<tr>
<td>
<code>status</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDStatus">
ArgoCDStatus
</a>
</em>
</td>
<td>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDApplicationControllerProcessorsSpec">ArgoCDApplicationControllerProcessorsSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDApplicationControllerSpec">ArgoCDApplicationControllerSpec</a>)
</p>
<p>
<p>ArgoCDApplicationControllerProcessorsSpec defines the options for the ArgoCD Application Controller processors.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>operation</code></br>
<em>
int32
</em>
</td>
<td>
<p>Operation is the number of application operation processors.</p>
</td>
</tr>
<tr>
<td>
<code>status</code></br>
<em>
int32
</em>
</td>
<td>
<p>Status is the number of application status processors.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDApplicationControllerSpec">ArgoCDApplicationControllerSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDApplicationControllerSpec defines the options for the ArgoCD Application Controller component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>processors</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDApplicationControllerProcessorsSpec">
ArgoCDApplicationControllerProcessorsSpec
</a>
</em>
</td>
<td>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDCASpec">ArgoCDCASpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDTLSSpec">ArgoCDTLSSpec</a>)
</p>
<p>
<p>ArgoCDCASpec defines the CA options for ArgCD.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>configMapName</code></br>
<em>
string
</em>
</td>
<td>
<p>ConfigMapName is the name of the ConfigMap containing the CA Certificate.</p>
</td>
</tr>
<tr>
<td>
<code>secretName</code></br>
<em>
string
</em>
</td>
<td>
<p>SecretName is the name of the Secret containing the CA Certificate and Key.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDCertificateSpec">ArgoCDCertificateSpec
</h3>
<p>
<p>ArgoCDCertificateSpec defines the options for the ArgoCD certificates.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>secretName</code></br>
<em>
string
</em>
</td>
<td>
<p>SecretName is the name of the Secret containing the Certificate and Key.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDDexOAuthSpec">ArgoCDDexOAuthSpec
</h3>
<p>
<p>ArgoCDDexOAuthSpec defines the desired state for the Dex OAuth configuration.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>enabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>Enabled will toggle OAuth support for the Dex server.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDDexSpec">ArgoCDDexSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDDexSpec defines the desired state for the Dex server component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>config</code></br>
<em>
string
</em>
</td>
<td>
<p>Config is the dex connector configuration.</p>
</td>
</tr>
<tr>
<td>
<code>image</code></br>
<em>
string
</em>
</td>
<td>
<p>Image is the Dex container image.</p>
</td>
</tr>
<tr>
<td>
<code>openShiftOAuth</code></br>
<em>
bool
</em>
</td>
<td>
<p>OpenShiftOAuth enables OpenShift OAuth authentication for the Dex server.</p>
</td>
</tr>
<tr>
<td>
<code>version</code></br>
<em>
string
</em>
</td>
<td>
<p>Version is the Dex container image tag.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDExport">ArgoCDExport
</h3>
<p>
<p>ArgoCDExport is the Schema for the argocdexports API</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>metadata</code></br>
<em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#objectmeta-v1-meta">
Kubernetes meta/v1.ObjectMeta
</a>
</em>
</td>
<td>
Refer to the Kubernetes API documentation for the fields of the
<code>metadata</code> field.
</td>
</tr>
<tr>
<td>
<code>spec</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportSpec">
ArgoCDExportSpec
</a>
</em>
</td>
<td>
<br/>
<br/>
<table>
<tr>
<td>
<code>argocd</code></br>
<em>
string
</em>
</td>
<td>
<p>ArgoCD is the name of the ArgoCD instance to export.</p>
</td>
</tr>
<tr>
<td>
<code>schedule</code></br>
<em>
string
</em>
</td>
<td>
<p>Schedule in Cron format, see <a href="https://en.wikipedia.org/wiki/Cron">https://en.wikipedia.org/wiki/Cron</a>.</p>
</td>
</tr>
<tr>
<td>
<code>storage</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportStorageSpec">
ArgoCDExportStorageSpec
</a>
</em>
</td>
<td>
<p>Storage defines the storage configuration options.</p>
</td>
</tr>
</table>
</td>
</tr>
<tr>
<td>
<code>status</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportStatus">
ArgoCDExportStatus
</a>
</em>
</td>
<td>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDExportLocalStorageSpec">ArgoCDExportLocalStorageSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportStorageSpec">ArgoCDExportStorageSpec</a>)
</p>
<p>
<p>ArgoCDExportLocalStorageSpec defines the desired state for local storage.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>pvc</code></br>
<em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#persistentvolumeclaimspec-v1-core">
Kubernetes core/v1.PersistentVolumeClaimSpec
</a>
</em>
</td>
<td>
<p>PVC is the desired characteristics for a PersistentVolumeClaim.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDExportSpec">ArgoCDExportSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDExport">ArgoCDExport</a>)
</p>
<p>
<p>ArgoCDExportSpec defines the desired state of ArgoCDExport</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>argocd</code></br>
<em>
string
</em>
</td>
<td>
<p>ArgoCD is the name of the ArgoCD instance to export.</p>
</td>
</tr>
<tr>
<td>
<code>schedule</code></br>
<em>
string
</em>
</td>
<td>
<p>Schedule in Cron format, see <a href="https://en.wikipedia.org/wiki/Cron">https://en.wikipedia.org/wiki/Cron</a>.</p>
</td>
</tr>
<tr>
<td>
<code>storage</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportStorageSpec">
ArgoCDExportStorageSpec
</a>
</em>
</td>
<td>
<p>Storage defines the storage configuration options.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDExportStatus">ArgoCDExportStatus
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDExport">ArgoCDExport</a>)
</p>
<p>
<p>ArgoCDExportStatus defines the observed state of ArgoCDExport</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>phase</code></br>
<em>
string
</em>
</td>
<td>
<p>Phase is a simple, high-level summary of where the ArgoCDExport is in its lifecycle.
There are five possible phase values:
Pending: The ArgoCDExport has been accepted by the Kubernetes system, but one or more of the required resources have not been created.
Running: All of the containers for the ArgoCDExport are still running, or in the process of starting or restarting.
Succeeded: All containers for the ArgoCDExport have terminated in success, and will not be restarted.
Failed: At least one container has terminated in failure, either exited with non-zero status or was terminated by the system.
Unknown: For some reason the state of the ArgoCDExport could not be obtained.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDExportStorageSpec">ArgoCDExportStorageSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportSpec">ArgoCDExportSpec</a>)
</p>
<p>
<p>ArgoCDExportStorageSpec defines the desired state for ArgoCDExport storage options.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>local</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDExportLocalStorageSpec">
ArgoCDExportLocalStorageSpec
</a>
</em>
</td>
<td>
<p>Local defines options for storage local to the cluster.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDGrafanaSpec">ArgoCDGrafanaSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDGrafanaSpec defines the desired state for the Grafana server component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>enabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>Enabled will toggle Grafana support globally for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>host</code></br>
<em>
string
</em>
</td>
<td>
<p>Host is the hostname to use for Ingress/Route resources.</p>
</td>
</tr>
<tr>
<td>
<code>image</code></br>
<em>
string
</em>
</td>
<td>
<p>Image is the Grafana container image.</p>
</td>
</tr>
<tr>
<td>
<code>size</code></br>
<em>
int32
</em>
</td>
<td>
<p>Size is the replica count for the Grafana Deployment.</p>
</td>
</tr>
<tr>
<td>
<code>version</code></br>
<em>
string
</em>
</td>
<td>
<p>Version is the Grafana container image tag.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDImportSpec">ArgoCDImportSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDImportSpec defines the desired state for the ArgoCD import/restore process.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>name</code></br>
<em>
string
</em>
</td>
<td>
<p>Name of an ArgoCDExport from which to import data.</p>
</td>
</tr>
<tr>
<td>
<code>namespace</code></br>
<em>
string
</em>
</td>
<td>
<p>Namespace for the ArgoCDExport, defaults to the same namespace as the ArgoCD.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDIngressSpec">ArgoCDIngressSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDIngressSpec defines the desired state for the Ingress resources.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>annotations</code></br>
<em>
map[string]string
</em>
</td>
<td>
<p>Annotations is the map of annotations to use for the Ingress resource.</p>
</td>
</tr>
<tr>
<td>
<code>enabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>Enabled will toggle Ingress support globally for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>path</code></br>
<em>
string
</em>
</td>
<td>
<p>Path is the path to use for the Ingress resource.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDPrometheusSpec">ArgoCDPrometheusSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDPrometheusSpec defines the desired state for the Prometheus component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>enabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>Enabled will toggle Prometheus support globally for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>host</code></br>
<em>
string
</em>
</td>
<td>
<p>Host is the hostname to use for Ingress/Route resources.</p>
</td>
</tr>
<tr>
<td>
<code>size</code></br>
<em>
int32
</em>
</td>
<td>
<p>Size is the replica count for the Prometheus StatefulSet.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDRBACSpec">ArgoCDRBACSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDRBACSpec defines the desired state for the Argo CD RBAC configuration.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>policy</code></br>
<em>
string
</em>
</td>
<td>
<p>Policy is CSV containing user-defined RBAC policies and role definitions.
Policy rules are in the form:
p, subject, resource, action, object, effect
Role definitions and bindings are in the form:
g, subject, inherited-subject
See <a href="https://github.com/argoproj/argo-cd/blob/master/docs/operator-manual/rbac.md">https://github.com/argoproj/argo-cd/blob/master/docs/operator-manual/rbac.md</a> for additional information.</p>
</td>
</tr>
<tr>
<td>
<code>defaultPolicy</code></br>
<em>
string
</em>
</td>
<td>
<p>DefaultPolicy is the name of the default role which Argo CD will falls back to, when
authorizing API requests (optional). If omitted or empty, users may be still be able to login,
but will see no apps, projects, etc&hellip;</p>
</td>
</tr>
<tr>
<td>
<code>scopes</code></br>
<em>
string
</em>
</td>
<td>
<p>Scopes controls which OIDC scopes to examine during rbac enforcement (in addition to <code>sub</code> scope).
If omitted, defaults to: &lsquo;[groups]&rsquo;.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDRedisSpec">ArgoCDRedisSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDRedisSpec defines the desired state for the Redis server component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>image</code></br>
<em>
string
</em>
</td>
<td>
<p>Image is the Redis container image.</p>
</td>
</tr>
<tr>
<td>
<code>version</code></br>
<em>
string
</em>
</td>
<td>
<p>Version is the Redis container image tag.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDServerGRPCSpec">ArgoCDServerGRPCSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerSpec">ArgoCDServerSpec</a>)
</p>
<p>
<p>ArgoCDServerGRPCSpec defines the desired state for the Argo CD Server GRPC options.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>host</code></br>
<em>
string
</em>
</td>
<td>
<p>Host is the hostname to use for Ingress/Route resources.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDServerServiceSpec">ArgoCDServerServiceSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerSpec">ArgoCDServerSpec</a>)
</p>
<p>
<p>ArgoCDServerServiceSpec defines the Service options for Argo CD Server component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>type</code></br>
<em>
<a href="https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.13/#servicetype-v1-core">
Kubernetes core/v1.ServiceType
</a>
</em>
</td>
<td>
<p>Type is the ServiceType to use for the Service resource.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDServerSpec">ArgoCDServerSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDServerSpec defines the options for the ArgoCD Server component.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>grpc</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerGRPCSpec">
ArgoCDServerGRPCSpec
</a>
</em>
</td>
<td>
<p>GRPC defines the state for the Argo CD Server GRPC options.</p>
</td>
</tr>
<tr>
<td>
<code>host</code></br>
<em>
string
</em>
</td>
<td>
<p>Host is the hostname to use for Ingress/Route resources.</p>
</td>
</tr>
<tr>
<td>
<code>insecure</code></br>
<em>
bool
</em>
</td>
<td>
<p>Insecure toggles the insecure flag.</p>
</td>
</tr>
<tr>
<td>
<code>service</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerServiceSpec">
ArgoCDServerServiceSpec
</a>
</em>
</td>
<td>
<p>Service defines the options for the Service backing the ArgoCD Server component.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCD">ArgoCD</a>)
</p>
<p>
<p>ArgoCDSpec defines the desired state of ArgoCD</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>applicationInstanceLabelKey</code></br>
<em>
string
</em>
</td>
<td>
<p>ApplicationInstanceLabelKey</p>
</td>
</tr>
<tr>
<td>
<code>configManagementPlugins</code></br>
<em>
string
</em>
</td>
<td>
<p>ConfigManagementPlugins is used to specify additional config management plugins.</p>
</td>
</tr>
<tr>
<td>
<code>controller</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDApplicationControllerSpec">
ArgoCDApplicationControllerSpec
</a>
</em>
</td>
<td>
<p>Controller defines the Application Controller options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>dex</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDDexSpec">
ArgoCDDexSpec
</a>
</em>
</td>
<td>
<p>Dex defines the Dex server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>gaTrackingID</code></br>
<em>
string
</em>
</td>
<td>
<p>GATrackingID is the google analytics tracking ID to use.</p>
</td>
</tr>
<tr>
<td>
<code>gaAnonymizeUsers</code></br>
<em>
bool
</em>
</td>
<td>
<p>GAAnonymizeUsers toggles user IDs being hashed before sending to google analytics.</p>
</td>
</tr>
<tr>
<td>
<code>grafana</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDGrafanaSpec">
ArgoCDGrafanaSpec
</a>
</em>
</td>
<td>
<p>Grafana defines the Grafana server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>helpChatURL</code></br>
<em>
string
</em>
</td>
<td>
<p>HelpChatURL is the URL for getting chat help, this will typically be your Slack channel for support.</p>
</td>
</tr>
<tr>
<td>
<code>helpChatText</code></br>
<em>
string
</em>
</td>
<td>
<p>HelpChatText is the text for getting chat help, defaults to &ldquo;Chat now!&rdquo;</p>
</td>
</tr>
<tr>
<td>
<code>image</code></br>
<em>
string
</em>
</td>
<td>
<p>Image is the ArgoCD container image for all ArgoCD components.</p>
</td>
</tr>
<tr>
<td>
<code>import</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDImportSpec">
ArgoCDImportSpec
</a>
</em>
</td>
<td>
<p>Import is the import/restore options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>ingress</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDIngressSpec">
ArgoCDIngressSpec
</a>
</em>
</td>
<td>
<p>Ingress defines the Ingress options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>kustomizeBuildOptions</code></br>
<em>
string
</em>
</td>
<td>
<p>KustomizeBuildOptions is used to specify build options/parameters to use with <code>kustomize build</code>.</p>
</td>
</tr>
<tr>
<td>
<code>oidcConfig</code></br>
<em>
string
</em>
</td>
<td>
<p>OIDCConfig is the configuration as an alternative to dex.</p>
</td>
</tr>
<tr>
<td>
<code>prometheus</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDPrometheusSpec">
ArgoCDPrometheusSpec
</a>
</em>
</td>
<td>
<p>Prometheus defines the Prometheus server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>rbac</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDRBACSpec">
ArgoCDRBACSpec
</a>
</em>
</td>
<td>
<p>RBAC defines the RBAC configuration for Argo CD.</p>
</td>
</tr>
<tr>
<td>
<code>redis</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDRedisSpec">
ArgoCDRedisSpec
</a>
</em>
</td>
<td>
<p>Redis defines the Redis server options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>repositories</code></br>
<em>
string
</em>
</td>
<td>
<p>Repositories to configure Argo CD with.</p>
</td>
</tr>
<tr>
<td>
<code>resourceCustomizations</code></br>
<em>
string
</em>
</td>
<td>
<p>ResourceCustomizations customizes resource behavior. Keys are in the form: group/Kind.</p>
</td>
</tr>
<tr>
<td>
<code>resourceExclusions</code></br>
<em>
string
</em>
</td>
<td>
<p>ResourceExclusions is used to completely ignore entire classes of resource group/kinds.</p>
</td>
</tr>
<tr>
<td>
<code>server</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDServerSpec">
ArgoCDServerSpec
</a>
</em>
</td>
<td>
<p>Server defines the options for the ArgoCD Server component.</p>
</td>
</tr>
<tr>
<td>
<code>sshKnownHosts</code></br>
<em>
string
</em>
</td>
<td>
<p>SSHKnownHosts defines the SSH known hosts data for connecting Git repositories via SSH.</p>
</td>
</tr>
<tr>
<td>
<code>statusBadgeEnabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>StatusBadgeEnabled toggles application status badge feature.</p>
</td>
</tr>
<tr>
<td>
<code>tls</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDTLSSpec">
ArgoCDTLSSpec
</a>
</em>
</td>
<td>
<p>TLS defines the TLS options for ArgoCD.</p>
</td>
</tr>
<tr>
<td>
<code>usersAnonymousEnabled</code></br>
<em>
bool
</em>
</td>
<td>
<p>UsersAnonymousEnabled toggles anonymous user access.
The anonymous users get default role permissions specified argocd-rbac-cm.</p>
</td>
</tr>
<tr>
<td>
<code>version</code></br>
<em>
string
</em>
</td>
<td>
<p>Version is the tag to use with the ArgoCD container image for all ArgoCD components.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDStatus">ArgoCDStatus
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCD">ArgoCD</a>)
</p>
<p>
<p>ArgoCDStatus defines the observed state of ArgoCD</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>phase</code></br>
<em>
string
</em>
</td>
<td>
<p>Phase is a simple, high-level summary of where the ArgoCD is in its lifecycle.
There are five possible phase values:
Pending: The ArgoCD has been accepted by the Kubernetes system, but one or more of the required resources have not been created.
Running: All of the containers for the ArgoCD are running, or in the process of starting or restarting.
Failed: At least one container has terminated in failure, either exited with non-zero status or was terminated by the system.
Unknown: For some reason the state of the ArgoCD could not be obtained.</p>
</td>
</tr>
</tbody>
</table>
<h3 id="argoproj.io/v1alpha1.ArgoCDTLSSpec">ArgoCDTLSSpec
</h3>
<p>
(<em>Appears on:</em>
<a href="#argoproj.io/v1alpha1.ArgoCDSpec">ArgoCDSpec</a>)
</p>
<p>
<p>ArgoCDTLSSpec defines the TLS options for ArgCD.</p>
</p>
<table>
<thead>
<tr>
<th>Field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>
<code>ca</code></br>
<em>
<a href="#argoproj.io/v1alpha1.ArgoCDCASpec">
ArgoCDCASpec
</a>
</em>
</td>
<td>
<p>CA defines the CA options.</p>
</td>
</tr>
<tr>
<td>
<code>certs</code></br>
<em>
map[string]string
</em>
</td>
<td>
<p>Certs defines custom TLS certificates for connecting Git repositories via HTTPS.</p>
</td>
</tr>
</tbody>
</table>
<hr/>
<p><em>
Generated with <code>gen-crd-api-reference-docs</code>
on git commit <code>4ff4739</code>.
</em></p>

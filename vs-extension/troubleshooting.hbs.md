# Troubleshoot Tanzu Developer Tools for Visual Studio

This topic tells you how to troubleshoot issues you encounter with
VMware Tanzu Developer Tools for Visual Studio.

## <a id="stop-button"></a> Stop button causes workload to fail

### Symptom

Clicking the red square Stop button in the Visual Studio top toolbar causes the
Tanzu Application Platform workload to fail or become unresponsive indefinitely.

### Solution

Do not click the button. Instead, in the top menu click **Debug** > **Detach All**.
A fix for this issue is planned for a future release.

### Symptom

Tanzu Workloads panel show "waiting on language server..."

### Solution

The language server has not started.  Open `workload.yaml` or `Tiltfile` in the editor.

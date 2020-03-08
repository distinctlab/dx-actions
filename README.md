# dx-actions

## **Inputs**

### **`private_action`**

**Required**

### **`action_path`**

**Optional**

## **Examples**

## Example usage

```yaml
- uses: distinctlab/dx-actions
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  with:
    private_action: distinctlab/dx-actions-webhook@master
    job_name: 'test'
    job_status: ${{ job.status }}
    next_job: 'build' #Optional
    run_id: ${{ github.run_id }}
    job_payload: '{ "version": "0.0.1", "url": "" }' #Optional
    pipeline_id: dx-actions-webhook
```

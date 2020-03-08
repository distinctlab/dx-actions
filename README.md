# dx-actions
 
## **Inputs**

### **`TOKEN`**
**Required**

### **`REPO`**
**Required**

### **`ACTION-PATH`**
**Optional**

## **Examples**

## Example usage

```yaml
- uses: distinctlab/dx-actions
  with:
    TOKEN: ${{ secrets.GITHUB_TOKEN }}
    REPO: distinctlab/dx-actions-webhook
    JOB_NAME: 'test'
    JOB_STATUS: ${{ job.status }}
    NEXT_JOB: 'build' #Optional
    RUN_ID: ${{ github.run_id }}
    JOB_PAYLOAD: '{ "version": "0.0.1", "url": "" }' #Optional
    PIPELINE_ID: dx-webhook
```

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
    TOKEN: ${{ secrets.TOKEN }}
    REPO: disttinctlab/dx-actions-webhook
    JOB_NAME: 'test'
    JOB_STATUS: ${{ job.status }}
    RUN_ID: ${{ github.run_id }}
    PIPELINE_ID: dx-webhook
```

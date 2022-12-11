---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlanRollbackBoundaryEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanRollbackBoundary» 
## Properties
| Property | Description |
| ------ | ----------- |
| [RecommendedTransaction](#recommendedtransaction) | Whether or not the rollback boundary was authored to use an MSI transaction. |
| [RollbackBoundaryId](#rollbackboundaryid) | Gets the identity of the rollback boundary to plan for. |
| [Transaction](#transaction) | Whether or not an MSI transaction will be used in the rollback boundary. If «see P:WixToolset.Mba.Core.PlanRollbackBoundaryEventArgs.RecommendedTransaction» is false, setting the value to true has no effect. If «see P:WixToolset.Mba.Core.PlanRollbackBoundaryEventArgs.RecommendedTransaction» is true, setting the value to false will cause the packages inside this rollback boundary to be executed without a wrapping MSI transaction. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## RecommendedTransaction Property {#recommendedtransaction}
Whether or not the rollback boundary was authored to use an MSI transaction.
### Declaration
```cs
public bool RecommendedTransaction { get; set; } 
```
## RollbackBoundaryId Property {#rollbackboundaryid}
Gets the identity of the rollback boundary to plan for.
### Declaration
```cs
public string RollbackBoundaryId { get; set; } 
```
## Transaction Property {#transaction}
Whether or not an MSI transaction will be used in the rollback boundary. If «see P:WixToolset.Mba.Core.PlanRollbackBoundaryEventArgs.RecommendedTransaction» is false, setting the value to true has no effect. If «see P:WixToolset.Mba.Core.PlanRollbackBoundaryEventArgs.RecommendedTransaction» is true, setting the value to false will cause the packages inside this rollback boundary to be executed without a wrapping MSI transaction.
### Declaration
```cs
public bool Transaction { get; set; } 
```

---
title: "<faultPropagationQuery>"
ms.date: "03/30/2017"
ms.topic: "reference"
ms.assetid: 4fb5c2b1-3dad-4eca-9c7f-3efb51899813
---

# \<faultPropagationQuery>

Represents a query that is used to track the handling of faults that occur within an activity.  This event occurs each time a FaultHandler processes a fault. You should use such query to track the handling of faults that occur within an activity. The query is necessary for a  tracking participant to subscribe to fault propagation records.

 For more information on tracking profile queries, see [Tracking Profiles](../../../windows-workflow-foundation/tracking-profiles.md).

\<system.serviceModel>\
\<tracking>\
\<trackingProfile>\
\<workflow>\
\<faultPropagationQueries>\
\<faultPropagationQuery>

## Syntax

```xml
<tracking>
  <trackingProfile name="Name">
    <workflow>
      <faultPropagationQueries>
        <faultPropagationQuery activityName="String"
                               faultHandlerActivityName="String" />
      </faultPropagationQueries>
    </workflow>
  </trackingProfile>
</tracking>
```

## Attributes and Elements

The following sections describe attributes, child elements, and parent elements.

### Attributes

|Attribute|Description|
|---------------|-----------------|
|activityName|A string that specifies the name of the fault handler activity that propagated the fault. The default is *, which indicates that fault propagation records are returned for all activities.|
|faultHandlerActivityName|A string that specifies the name of the activity that was the source of the fault.|

### Child Elements

None.

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[\<faultPropagationQueries>](faultpropagationqueries.md)|Represents a list of configuration elements that are used to track the handling of faults that occur within an activity.  This event occurs each time a FaultHandler processes a fault.|

## See also

- <xref:System.ServiceModel.Activities.Tracking.Configuration.FaultPropagationQueryElement?displayProperty=nameWithType>
- <xref:System.Activities.Tracking.FaultPropagationQuery?displayProperty=nameWithType>
- [Workflow Tracking and Tracing](../../../windows-workflow-foundation/workflow-tracking-and-tracing.md)
- [Tracking Profiles](../../../windows-workflow-foundation/tracking-profiles.md)

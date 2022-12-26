---
title: SSMS Options page - Output Window
description: SSMS Options (Output Window)
author: erinstellato-ms
ms.author: erinstellato
ms.reviewer: maghan
ms.date: 12/19/2022
ms.service: sql
ms.subservice: ssms
ms.topic: ui-reference
f1_keywords:
  - "VS.ToolsOptionsPages.Query_Execution.Sql_Server.General"
dev_langs:
  - TSQL
---

# Options (Output Window - General)

[!INCLUDE[SQL Server Azure SQL Database PDW](../../includes/applies-to-version/sql-asdb-asdbmi-pdw.md)]

Use this page to set the default behavior of the output window. To access the settings, on the **Tools** menu, select **Options**, and expand the **Output Window** folder.

## Log Channels

Four logging channels are available to provide more information when using SQL Server Management Studio.

| Channel | Definition |
| --- | --- |
| Object Explorer | This channel outputs the query text and elapsed times of SQL queries needed to expand nodes in Object Explorer. Each query logs a Begin Query and an End Query event. Each event has a timestamp and the URN associated with the entity being queried. The URN refers to the underlying SQL Management Object and consists of an XPath-style hierarchy. For example, the URN for a table named "Table1" in database "Db" on server "MyServer" would be "Server[@Name='MyServer']/Database[@Name='Db']/Table[/@Name='Table1']". Expanding one node in Object Explorer can require multiple such queries with different parameters. The End Query event will contain the elapsed time of the query along with the T-SQL text. You may find this query data useful for server performance analysis in cases where Object Explorer seems unusually slow to expand a particular node. Note: only some nodes in Object Explorer provide this query detail when expanding. Enabled by default. |
| Telemetry | Telemetry is the stream of anonymous feature usage data collected by Microsoft. These events could be useful for your tracking of SSMS usage. It can help you identify what Object Explorer nodes you expand and what commands run during your SSMS session while the Output window is open. Enabled by default. |
| SQL Client | This channel displays information from the Microsoft.Data.SqlClient data provider. This option requires a restart of SSMS for output to appear. |
| Azure Activity Directory Interactive authentication | For cases where Azure Active Directory authentication is used, this channel will output information specific to the authentication process. |

## Next steps

- [Query execution options](options-query-execution.md)
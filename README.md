# `DROP_PROCEDURE_IF_EXISTS`

A simple procedure to help simulating `ALTER` procedure for T-SQL (SQL Server). In Oracle, you can do `CREATE OR ALTER PROCEDURE`, while in SQL Server, you must drop it. This procedure solves this problem by conditionally deleting the procedure in order to replace it later.

## Installation

Run the content under `DROP_PROCEDURE_IF_EXISTS` in your database.

## Usage

`EXEC DROP_PROCEDURE_IF_EXISTS [PROC_NAME]`

## Example

```sql
EXEC DROP_PROCEDURE_IF_EXISTS [PROC_CREATE_USER]
GO

CREATE PROCEDURE [dbo].[PROC_CREATE_USER]
  @NAME VARCHAR(255)
  ...
```

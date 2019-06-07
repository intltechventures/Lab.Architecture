
# Batch Best Practices

## 1. Introduction


## 2. Batch Domain Model

### 2.1 Job

### 2.2 Step

### 2.3 Item

### 2.4 Reader

### 2.5 Writer

### 2.6 Process

## 3. Batch Patterns & Concepts

### 3.1 Pattern: Batch Control File

### 3.2 Pattern: Header-Footer

### 2.3 Pattern: Single-Line Item Records

### 2.4 Pattern: Multi-Line Item Records

### 2.5 Pattern: Parallel Item Processing

### 2.6 Pattern: Chunking

### 2.7 Pattern: All-or-None

### 2.8 Pattern: Error Threshhold 

### 2.9 Pattern: Rejected-Recovery


## 4. Technology Selection

### 4.1 ETL Tools

### 4.2 Vendor Supplied APIs

### 4.3 Apache Camel (Java)

### 4.4 Spring Batch (Java)

## 5 Job Scheduling

### 5.1 Quartz

### 5.2 CA Workload Automation AE (AutoSys Edition)
- https://en.wikipedia.org/wiki/CA_Workload_Automation_AE

## 6. Job Monitoring

### 6.1 HP OpenView 


## 7. Logging

### 7.1 Logging Events

#### 7.1.1 Batch Job Started

#### 7.1.2 Data: File {Source | Target} Processed
- {Source | Target} File [name] Processed
- {Source | Target} [#] Total Records Processed
- {Source | Target} [#] Records Successfully Processed
- {Source | Target} [#] Records Rejected/Skipped with Errors

#### 7.1.3 Data: API {Source | Target} Processed

#### 7.1.4 Data: Stream {Source | Target} Processed

#### 7.1.5 Data: Event {Source | Starget} Processed

#### 7.1.6 Data: Queue {Source | Target} Processed

#### 7.1.7 Batch Job Aborted

#### 7.1.8 Batch Job Completed
- Job Stats
  + [#] {Records | Events} Successfully Processed
  + [#] {Records | Events} Rejected/Skipped with Errors


## 8. Processing Inbound Files

### 8.1 Log "FILE PROCESSED" Event

### 8.2 Archiving Inbound Files


## 9. Processing Outbound Files

### 9.1 Processing Outbound Files

### 9.2 Archiving Outbound Files


## 10. Batch Process/Application Design

### 10.1 General Flow


### 10.2 Common Batch Processing Patterns
- Transactional
- Full Extract
- Delta Extract (i.e. Changes Only) 
- Merge
- Filter
- Annotate/Enrich
- Sort
- Import
- Apply Deltas
- Apply Fix/Adjustment
- Purge/Delete


### 10.2 Class Model

### 10.3 Activity Diagram

### 10.4 Configuration

### 10.5 Restart/Recoverability


## 12. File Delivery Mechanisms & Processes

### 12.1 SFTP
- Axway
- IBM Sterling MFT
- Ipswitch File Transfer (MOVE.it) 
- Tibco MFT 


### 12.2 AWS S3

### 12.3 Azure Storage

### 12.4 Google Drive 

### 12.5 Box.com

### 12.6 DropBox.com 



## 13. Batch Security

### 13.1 Encryption-at-Rest

### 13.2 Encryption-in-Transit
- GNU PGP Encryption

### 13.3 Encryption Key Management


## 14. Batch Governance/Controls
- Questions that the Batch Architture needs to support answering:
  + When was the last time this interface was executed?
  + How many records/events were processed during a specific run?
  + How many records were rejected during a specific run?
  + How long did it take for this interface to execute for a specific run?
  + Are there any interfaces that are currently executing?
  + Are there any interfaces that have aborted?
  + What are the specific details of the last aborted interface?
  + For a specified "Expected Duration" parameter, for any given batch job: 
    * How often has the job exceeded that expected duration?
    * What are the specific details of the previous execution instances?
  + What are the trendlines for a given interface (e.g. execution duration, number of records processed, size of data inputs/outputs)?
    * Has the trendline demonstrated a move of a magnitude greater than [x] - over a [y] period - for the monitored aspect [z]?
      * If so, trigger an alert to notify Operations
  + Has this job already processed this input file during some previous run?
  + If this input file has been processed before, has an explicit override been passed to the batch job to override duplicate processing prevention mechanisms?


## 15. Batch Job Design Considerations

### 15.1 Batch vs. Real-Time

### 15.2 Disadvantage of Batch Processing

### 15.3 Advantages of Batch Processing







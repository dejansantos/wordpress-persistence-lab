# Root Cause Analysis

## Investigation Steps

### 1. Network validation
Used debug container to verify connectivity.

### 2. Storage inspection
Checked WordPress upload directory:
 /var/www/html/wp-content/uploads

### 3. Container lifecycle analysis
Observed that data existed only inside container filesystem.

## Root Cause
WordPress uploads were stored in ephemeral container storage,
which is destroyed when containers are removed.

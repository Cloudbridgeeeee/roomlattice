# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Booking exports, guest names removed as they arrive |
| SageMaker AI | Occupancy and housekeeping demand models per property |
| Bedrock | Plain-language daily plans that quote their figures |
| DynamoDB | Rooms, shifts, plans and the decision log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.

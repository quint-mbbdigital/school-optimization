# School Performance Dashboard API Endpoints

## Authentication Endpoints

1. `POST /api/auth/login`
   - Authenticates user credentials
   - Returns a JWT token for subsequent requests

2. `POST /api/auth/logout`
   - Invalidates the current user's session

3. `GET /api/auth/user`
   - Retrieves the current user's profile information

## School Information Endpoints

4. `GET /api/schools`
   - Retrieves a list of all schools
   - Supports pagination and filtering

5. `GET /api/schools/{schoolId}`
   - Retrieves detailed information for a specific school

## Performance Metrics Endpoints

6. `GET /api/performance/{schoolId}`
   - Retrieves overall performance metrics for a specific school
   - Includes academic, social-emotional, and teacher quality scores

7. `GET /api/performance/{schoolId}/academic`
   - Retrieves detailed academic performance metrics
   - Includes standardized test scores, graduation rates, etc.

8. `GET /api/performance/{schoolId}/social-emotional`
   - Retrieves social-emotional learning metrics
   - Includes student engagement scores, behavioral incident rates, etc.

9. `GET /api/performance/{schoolId}/teacher-quality`
   - Retrieves teacher quality metrics
   - Includes teacher qualifications, retention rates, etc.

## Time Series Data Endpoints

10. `GET /api/timeseries/{schoolId}`
    - Retrieves historical performance data for a school
    - Supports date range parameters

11. `GET /api/timeseries/compare`
    - Retrieves comparative time series data for multiple schools
    - Accepts multiple school IDs as parameters

## Event and Intervention Endpoints

12. `GET /api/events/{schoolId}`
    - Retrieves significant events and interventions for a school
    - Supports date range parameters

13. `POST /api/events/{schoolId}`
    - Adds a new event or intervention for a school

14. `GET /api/events/{schoolId}/{eventId}`
    - Retrieves detailed information about a specific event

## Resource Allocation Endpoints

15. `GET /api/resources/{schoolId}`
    - Retrieves current resource allocation data for a school

16. `POST /api/resources/{schoolId}/simulate`
    - Simulates the impact of resource reallocation
    - Accepts proposed changes as parameters

## Predictive Analytics Endpoints

17. `GET /api/predict/{schoolId}`
    - Retrieves performance predictions for a school

18. `POST /api/predict/scenario`
    - Generates predictions based on hypothetical scenarios
    - Accepts various parameters for the scenario

## Comparison Endpoints

19. `GET /api/compare`
    - Retrieves comparative data for multiple schools
    - Accepts multiple school IDs and metrics as parameters

## Demographic Data Endpoints

20. `GET /api/demographics/{schoolId}`
    - Retrieves demographic data for a specific school

21. `GET /api/demographics/district/{districtId}`
    - Retrieves aggregated demographic data for a district

## Financial Data Endpoints

22. `GET /api/finance/{schoolId}`
    - Retrieves financial data for a specific school
    - Includes budget information, per-student spending, etc.

## Extracurricular Data Endpoints

23. `GET /api/extracurricular/{schoolId}`
    - Retrieves data on extracurricular activities
    - Includes participation rates, types of activities, etc.

## College and Career Readiness Endpoints

24. `GET /api/ccr/{schoolId}`
    - Retrieves college and career readiness metrics
    - Includes college acceptance rates, career program participation, etc.

## Report Generation Endpoints

25. `POST /api/reports/generate`
    - Generates a comprehensive report based on specified parameters
    - Returns a link to download the report

## Data Export Endpoints

26. `GET /api/export/{dataType}`
    - Exports specified data in various formats (CSV, JSON, etc.)
    - Supports parameters for customizing the export

## Feedback and Rating Endpoints

27. `POST /api/feedback`
    - Submits user feedback on the dashboard or specific features

28. `GET /api/ratings/{schoolId}`
    - Retrieves community ratings and feedback for a school

## System Health and Metadata Endpoints

29. `GET /api/system/health`
    - Retrieves the current system status and health metrics

30. `GET /api/metadata`
    - Retrieves metadata about available metrics, data sources, etc.
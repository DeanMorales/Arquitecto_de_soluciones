# Dominio 1: Design Secure Architectures (30%)

## Descripción General del Dominio

El **Dominio 1: Design Secure Architectures** constituye el área de mayor peso en el examen de certificación AWS Solutions Architect Associate (SAA-C03), representando el **30% de la puntuación total**. Este dominio evalúa la capacidad del candidato para diseñar arquitecturas seguras que protejan datos, gestionen el acceso y cumplan con los requisitos de seguridad en la nube de AWS.

La seguridad en AWS se fundamenta en el **modelo de responsabilidad compartida**, donde AWS es responsable de la seguridad *de* la nube (infraestructura física, redes, hypervisor), mientras que el cliente es responsable de la seguridad *en* la nube (datos, configuraciones, identidad, aplicaciones).

Este dominio requiere un entendimiento profundo de:
- Principios de seguridad de AWS
- Servicios de identidad y acceso (IAM)
- Configuración de redes seguras (VPC)
- Protección de datos (cifrado)
- Servicios de seguridad avanzados

---

## Task 1.1: Design Secure Access to AWS Resources

### Descripción
Disenar el acceso seguro a los recursos de AWS implica implementar controles de identidad robustos que garanticen que solo usuarios y servicios autorizados puedan interactuar con los recursos de la nube, siguiendo el principio de mínimo privilegio.

### Conocimientos Requeridos (Knowledge)

- **Infraestructura global de AWS**: Comprender cómo las Availability Zones y AWS Regions afectan el diseño de arquitecturas seguras.
- **Mejores prácticas de seguridad de AWS**: Aplicar el principio de mínimo privilegio (least privilege).
- **Modelo de responsabilidad compartida de AWS**: Entender qué responsabilidades tiene AWS vs. el cliente.

### Habilidades Requeridas (Skills)

#### 1. Aplicar mejores prácticas de seguridad a usuarios IAM y root
- Implementar **Multi-Factor Authentication (MFA)** para el usuario root
- Configurar MFA para usuarios IAM críticos
- Utilizar contraseñas fuertes y políticas de contraseñas
- Rotar credenciales regularmente

#### 2. Diseñar un modelo de autorización flexible
- **IAM Users**: Para acceso programático y Console permanente
- **IAM Groups**: Para organizar permisos por rol/Departamento
- **IAM Roles**: Para acceso temporal y servicios
- **IAM Policies**: JSON para definir permisos específicos

#### 3. Diseñar estrategia de control de acceso basada en roles
- **AWS STS (Security Token Service)**: Emitir credenciales temporales
- **Role Switching**: Permitir a usuarios cambiar entre roles
- **Cross-Account Access**: Acceso entre cuentas AWS
- ** federation**: Integrar directorios corporativos

#### 4. Diseñar estrategia de seguridad para múltiples cuentas AWS
- **AWS Control Tower**: Governance centralizada de múltiples cuentas
- **Service Control Policies (SCPs)**: Restringir servicios a nivel de organización
- **AWS Organizations**: Estructura jerárquica de cuentas
- **AWS SSO / IAM Identity Center**: Acceso unificado

#### 5. Determinar uso apropiado de políticas de recursos
- Resource-based policies vs. Identity-based policies
- Bucket policies para S3
- Role trust policies
- Lambda function policies

#### 6. Determinar cuándo federar servicios de directorio con roles IAM
- **AWS IAM Identity Center**: SSO integrado con Okta, Azure AD
- **SAML 2.0**: Federación con Microsoft Active Directory
- **Web Identity Federation**: Para aplicaciones móvil/web

### Servicios Clave
- IAM (Users, Groups, Roles, Policies)
- AWS STS
- AWS Organizations
- AWS Control Tower
- IAM Identity Center
- AWS Directory Service

---

## Task 1.2: Design Secure Workloads and Applications

### Descripción
Disenar cargas de trabajo y aplicaciones seguras implica proteger la infraestructura computacional, las aplicaciones y los datos que residen en AWS, considerando amenazas externas e internas.

### Conocimientos Requeridos (Knowledge)

- **Seguridad de configuración de aplicaciones y credenciales**: Gestión segura de secrets, credenciales de base de datos, claves API.
- **Endpoints de servicios de AWS**: Comprender los diferentes tipos de endpoints.
- **Control de puertos, protocolos y tráfico de red**: Configuración de seguridad de red.
- **Acceso seguro a aplicaciones**: Autenticación y autorización a nivel de aplicación.
- **Servicios de seguridad con casos de uso apropiados**:
  - **AWS Cognito**: Autenticación de usuarios
  - **AWS GuardDuty**: Detección de amenazas
  - **AWS Macie**: Protección de datos sensibles
- **Vectores de amenazas externos**:
  - **DDoS**: Ataques de denegación de servicio
  - **SQL Injection**: Inyección de código en bases de datos
  - **XSS**: Cross-site scripting
  - **Man-in-the-Middle**: Intercepción de tráfico

### Habilidades Requeridas (Skills)

#### 1. Diseñar arquitecturas VPC con componentes de seguridad
- **Security Groups**: Firewall stateful a nivel de instancia
- **Route Tables**: Control de enrutamiento de tráfico
- **Network ACLs (NACLs)**: Firewall stateless a nivel de subred
- **NAT Gateways**: Permitir tráfico saliente desde subredes privadas
- **Internet Gateways**: Conectividad pública
- **VPC Endpoints**: Acceso a servicios AWS sin internet

#### 2. Determinar estrategias de segmentación de red
- **Subredes Públicas**: Para recursos que necesitan acceso a internet (ALB, NAT Gateway)
- **Subredes Privadas**: Para aplicaciones, bases de datos, servicios internos
- ** subredes de Datos**: Aislamiento adicional para datos sensibles
- **Arquitectura de capas**: DMZ, aplicación, datos

#### 3. Integrar servicios AWS para asegurar aplicaciones
- **AWS Shield**: Protección contra DDoS
- **AWS WAF**: Filtrado de tráfico web (OWASP Top 10)
- **AWS Secrets Manager**: Gestión de secretos
- **AWS Systems Manager Parameter Store**: Configuración segura

#### 4. Asegurar conexiones externas a y desde AWS
- **VPN**: Conexiones seguras sitio-a-sitio
- **AWS Direct Connect**: Conexión dedicada de alta velocidad
- **AWS Client VPN**: Acceso VPN para clientes
- **Security Groups**: Control de tráfico entrante/saliente

### Servicios Clave
- VPC (Virtual Private Cloud)
- Security Groups
- NACLs
- NAT Gateway / NAT Instance
- Internet Gateway
- VPC Endpoints (Interface & Gateway)
- AWS WAF / Shield
- AWS Secrets Manager
- AWS Cognito

---

## Task 1.3: Design Security for Edge Protection

### Descripción
Disenar seguridad para protección perimetral implica proteger las aplicaciones y servicios que están expuestos a internet, utilizando servicios de AWS para mitigar amenazas y optimizar la entrega de contenido.

### Conocimientos Requeridos (Knowledge)

- **Protección contra DDoS**: Comprender los tipos de ataques y contramedidas.
- **CDN y distribución de contenido**: CloudFront y Edge Locations.
- **DNS y enrutamiento**: Route 53 y sus características de seguridad.
- **Certificates**: Gestión de certificados SSL/TLS.
- **Web Application Firewall**: Reglas de filtrado para aplicaciones web.

### Habilidades Requeridas (Skills)

#### 1. Configurar protección contra ataques DDoS
- **AWS Shield Standard**: Protección básica automatizada
- **AWS Shield Advanced**: Protección avanzada con soporte 24/7
- **WAF Rules**: Reglas personalizadas contra ataques已知
- **Rate Limiting**: Limitar solicitudes por IP

#### 2. Implementar arquitectura de CDN segura
- **CloudFront Distributions**: Distribución de contenido con HTTPS
- **Origin Access Control (OAC)**: Proteger orígenes S3
- **Signed URLs/Cookies**: Control de acceso a contenido premium
- **Geo-restrictions**: Restringir contenido por ubicación

#### 3. Configurar DNS seguro
- **Route 53**: Resolver seguro con DNSSEC
- **Private Hosted Zones**: DNS interno privado
- **Health Checks**: Monitorización de disponibilidad

#### 4. Gestionar certificados SSL/TLS
- **AWS Certificate Manager (ACM)**: Certificados gratuitos
- **Certificate Renewal**: Renovación automática
- **Server Name Indication (SNI)**: Múltiples certificados

### Servicios Clave
- AWS Shield (Standard/Advanced)
- Amazon CloudFront
- AWS WAF
- Amazon Route 53
- AWS Certificate Manager (ACM)

---

## Task 1.4: Design Data Protection

### Descripción
Disenar protección de datos implica implementar mecanismos de cifrado, control de acceso y gestión de claves para proteger la información sensible en reposo y en tránsito.

### Conocimientos Requeridos (Knowledge)

- **Cifrado en reposo**: Datos almacenados en S3, EBS, RDS, DynamoDB.
- **Cifrado en tránsito**: TLS/SSL para comunicaciones.
- **Gestión de claves**: AWS KMS, CloudHSM.
- **Clasificación de datos**: Identificar datos sensibles (PII, PHI, financial).
- **Prevención de pérdida de datos (DLP)**: Servicios y estrategias.

### Habilidades Requeridas (Skills)

#### 1. Implementar cifrado en reposo
- **S3 Server-Side Encryption (SSE)**:
  - SSE-S3: Claves gestionadas por S3
  - SSE-KMS: Claves en AWS KMS (recomendado)
  - SSE-C: Claves proporcionadas por cliente
- **EBS Encryption**: Cifrado automático de volúmenes
- **RDS Encryption**: Cifrado de bases de datos
- **DynamoDB**: Cifrado en reposo con KMS

#### 2. Implementar cifrado en tránsito
- **TLS/SSL**: Certificados para servicios AWS
- **ACM**: Gestión de certificados
- **Elastic Load Balancing**: HTTPS listener
- **CloudFront**: HTTPS obligatorio

#### 3. Diseñar estrategia de gestión de claves
- **AWS KMS**:
  - Customer Managed Keys (CMK)
  - AWS Managed Keys
  - Claves personalizadas
- **CloudHSM**: Módulos de seguridad de hardware
- **Key Rotation**: Rotación automática de claves
- **Key Policies**: Control de acceso a claves

#### 4. Implementar controls de protección de datos
- **S3 Bucket Policies**: Control de acceso a nivel de bucket
- **Access Points**: Puntos de acceso especializados
- **Block Public Access**: Previene acceso público accidental
- **Versioning**: Protección contra eliminación
- **Replication**: Replicación entre regiones

#### 5. Gestionar datos sensibles
- **AWS Macie**: Descubrimiento automático de datos sensibles
- **Secrets Manager**: Credenciales de base de datos
- **Systems Manager Parameter Store**: Parámetros seguros

### Servicios Clave
- AWS KMS (Key Management Service)
- Amazon S3 (Encryption, Policies, Versioning)
- Amazon EBS (Encryption)
- Amazon RDS (Encryption)
- Amazon DynamoDB (Encryption)
- AWS Certificate Manager
- AWS Macie
- AWS Secrets Manager
- CloudHSM

---

## Task 1.5: Design Secure Applications

### Descripción
Disenar aplicaciones seguras implica integrar prácticas de seguridad en el ciclo de desarrollo de software, desde el diseño hasta el despliegue, considerando authentication, authorization y protección contra vulnerabilidades.

### Conocimientos Requeridos (Knowledge)

- **Application Security**: Seguridad a nivel de código y aplicación.
- **Authentication & Authorization**: Diferentes modelos y estrategias.
- **API Security**: Protección de interfaces de programación.
- **Microservices Security**: Seguridad en arquitecturas distribuidas.
- **DevSecOps**: Integración de seguridad en CI/CD.

### Habilidades Requeridas (Skills)

#### 1. Implementar autenticación segura
- **Amazon Cognito**:
  - User Pools: Autenticación de usuarios
  - Identity Pools: Acceso temporal a AWS
  - MFA: Autenticación multifactor
- **IAM Roles**: Para acceso de aplicaciones
- **OAuth 2.0 / OpenID Connect**: Estándares de industria

#### 2. Implementar autorización a nivel de aplicación
- **Attribute-Based Access Control (ABAC)**: Permisos basados en atributos
- **Resource-Based Policies**: Políticas en recursos
- **Lambda Authorizers**: Autorización custom para API Gateway

#### 3. Proteger APIs
- **API Gateway**:
  - API Keys: Control de acceso básico
  - Usage Plans: Limitación de uso
  - Lambda Authorizers: Autenticación custom
  - IAM Authorization: Firma de solicitudes v4
- **CORS**: Configuración segura de Cross-Origin

#### 4. Integrar seguridad en CI/CD
- **AWS CodePipeline**: Pipeline de integración segura
- **CodeBuild**: Builds en entornos aislados
- **CodeDeploy**: Despliegues seguros
- **Security Scanning**: Análisis de vulnerabilidades

#### 5. Proteger contra vulnerabilidades comunes
- **Input Validation**: Validación de datos de entrada
- **SQL Injection Prevention**: Uso de parameterized queries
- **Secrets Management**: No hardcodear credenciales
- **Logging & Monitoring**: Registro de actividades sospechosas

### Servicios Clave
- Amazon Cognito
- API Gateway
- AWS Lambda
- AWS CodePipeline / CodeBuild / CodeDeploy
- Amazon CloudWatch (Logs, Events)
- AWS X-Ray (Security Tracing)

---

## Ejercicios Prácticos: Proyectos Personales

A continuaciÃ³n se presentan tres arquitecturas de referencia para implementar como proyectos personales que te ayudarÃ¡n a consolidar los conceptos de seguridad en AWS.

---

### Proyecto 1: Arquitectura Web Segura con Alta Disponibilidad

#### Descripción del Proyecto
Desplegar una aplicaciÃ³n web segura y de alta disponibilidad que incluya:
- Web tier en subredes pÃºblicas
- Application tier en subredes privadas
- Base de datos en subredes privadas con cifrado
- Balanceador de carga seguro (HTTPS)
- ProtecciÃ³n contra DDoS y WAF
- AutenticaciÃ³n mediante Cognito

#### Arquitectura Sugerida

```
┌─────────────────────────────────────────────────────────────────┐
│                         INTERNET                                 │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    CLOUDFRONT + WAF + SHIELD                     │
│              (Edge Locations - Caché y Seguridad)               │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                APPLICATION LOAD BALANCER (ALB)                  │
│                    (SSL/TLS - HTTPS Only)                       │
└─────────────────────────────┬───────────────────────────────────┘
                              │
        ┌─────────────────────┴─────────────────────┐
        │                                             │
        ▼                                             ▼
┌───────────────────┐                     ┌───────────────────��
│   PUBLIC SUBNET   │                     │   PUBLIC SUBNET   │
│      (AZ 1)       │                     │      (AZ 2)       │
│                   │                     │                   │
│ ┌───────────────┐ │                     │ ┌───────────────┐ │
│ │  EC2 Web Tier │ │                     │ │  EC2 Web Tier │ │
│ │  (Auto Scale) │ │                     │ │  (Auto Scale) │ │
│ └───────────────┘ │                     │ └───────────────┘ │
└───────────────────┘                     └───────────────────┘
        │                                             │
        └─────────────────────┬──────────────────���──┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                    PRIVATE SUBNETS (APP TIER)                   │
│         ┌──────────────────┐      ┌──────────────────┐        │
│         │  Private Subnet  │      │  Private Subnet  │        │
│         │     (AZ 1)       │      │     (AZ 2)       │        │
│         │                  │      │                  │        │
│         │ ┌──────────────┐ │      │ ┌──────────────┐ │        │
│         │ │ EC2 App Tier │ │      │ │ EC2 App Tier │ │        │
│         │ └──────────────┘ │      │ └──────────────┘ │        │
│         └──────────────────┘      └──────────────────┘        │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                   PRIVATE SUBNETS (DATA TIER)                   │
│         ┌──────────────────┐      ┌──────────────────┐        │
│         │  Private Subnet  │      │  Private Subnet  │        │
│         │     (AZ 1)       │      │     (AZ 2)       │        │
│         │                  │      │                  │        │
│         │ ┌──────────────┐ │      │ ┌──────────────┐ │        │
│         │ │  RDS Aurora  │ │      │ │  RDS Aurora  │ │        │
│         │ │  (Encrypted) │ │      │ │  (Encrypted) │ │        │
│         │ └──────────────┘ │      │ └──────────────┘ │        │
│         └──────────────────┘      └──────────────────┘        │
└─────────────────────────────────────────────────────────────────┘
```

#### Componentes de Seguridad a Implementar

| Componente | Configuración de Seguridad |
|------------|----------------------------|
| **VPC** | Bloques CIDR apropiados (/16 para VPC, /20 para subredes) |
| **Security Groups** | Web Tier: 443/80 desde ALB; App Tier: 443 desde Web Tier; DB: 5432 desde App Tier |
| **NACLs** | Stateless filtering - permitir tráfico válido |
| **S3 Buckets** | Cifrado SSE-KMS, Versioning, Block Public Access |
| **RDS** | Encryption enabled, Multi-AZ, Automated backups |
| **Route 53** | Health checks, DNSSEC |
| **CloudFront** | OAC, HTTPS-only, WAF integration |

#### Pasos de Implementación

1. **Crear VPC** con 2 AZs, 6 subredes (2 públicas, 2 privadas app, 2 privadas data)
2. **Configurar Internet Gateway** y rutas
3. **Crear NAT Gateways** en subredes públicas
4. **Configurar Security Groups** con reglas restrictivas
5. **Desplegar ALB** con HTTPS listener (ACM)
6. **Configurar Auto Scaling Groups** para Web y App tiers
7. **Desplegar RDS** con cifrado y Multi-AZ
8. **Configurar CloudFront** con WAF
9. **Integrar Cognito** para autenticación de usuarios

---

### Proyecto 2: Pipeline de Datos Seguro con Serverless

#### Descripción del Proyecto
Construir un pipeline de procesamiento de datos que:
- Ingiera datos desde múltiples fuentes
- Procese datos de forma segura usando Lambda
- Almacene resultados en S3 con cifrado
- Implemente principios de mínimo privilegio
- Registre todas las operaciones para auditoría

#### Arquitectura Sugerida

```
┌─────────────────────────────────────────────────────────────────┐
│                        DATA SOURCES                              │
│    ┌─────────┐   ┌─────────┐   ┌─────────┐   ┌─────────┐       │
│    │   S3    │   │  Kinesis│   │   API   │   │   IoT   │       │
│    │ Upload  │   │  Stream │   │ Gateway │   │  Core   │       │
│    └────┬────┘   └────┬────┘   └────┬────┘   └────┬────┘       │
└─────────┼─────────────┼─────────────┼─────────────┼─────────────┘
          │             │             │             │
          ▼             ▼             ▼             ▼
┌─────────────────────────────────────────────────────────────────┐
│                      VPC ENDPOINTS                               │
│         (S3 Gateway Endpoint - Sin acceso a internet)          │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                     AWS LAMBDA FUNCTIONS                         │
│   ┌─────────────┐  ┌─────────────┐  ┌─────────────┐            │
│   │  Data       │  │  Data       │  │  Data       │            │
│   │  Ingestion  │─▶│  Processing │─▶│  Validation │            │
│   └─────────────┘  └─────────────┘  └─────────────┘            │
│         │                                    │                   │
│         │              IAM Role             │                   │
│         │         (Mínimo Privilegio)       │                   │
└─────────┼───────────────────────────────────┼───────────────────┘
          │                                   │
          ▼                                   ▼
┌─────────────────────────────────────────────────────────────────┐
│                    SECURE S3 BUCKETS                            │
│   ┌─────────────────────┐    ┌─────────────────────┐           │
│   │  raw-data-bucket    │    │  processed-data     │           │
│   │  (SSE-KMS + S3     │    │  -bucket            │           │
│   │   Block Public)    │    │  (SSE-KMS +        │           │
│   │  Versioning: ON    │    │   Versioning: ON)  │           │
│   └─────────────────────┘    └─────────────────────┘           │
└─────────────────────────────────────────────────────────────────┘
          │
          ▼
┌─────────────────────────────────────────────────────────────────┐
│                     CLOUDWATCH & CLOUDTRAIL                      │
│         (Logging, Monitoring, Audit Trail - Security)          │
└─────────────────────────────────────────────────────────────────┘
```

#### Componentes de Seguridad a Implementar

| Componente | Configuración de Seguridad |
|------------|----------------------------|
| **IAM Roles** | Least privilege para cada Lambda function |
| **VPC Endpoints** | Acceso a S3 sin internet pública |
| **S3 Buckets** | SSE-KMS, Bucket Policies restrictivas |
| **KMS Keys** | CMK con rotación habilitada |
| **Lambda** | Execution role específico por función |
| **CloudWatch** | Logs con retención apropiada |
| **CloudTrail** | Trail para auditoría de API calls |

#### Servicios y Características de Seguridad Clave

- **IAM Roles con políticas específicas**: Cada Lambda tiene solo los permisos necesarios
- **VPC Endpoints (Gateway)**: Comunicación privada con S3
- **SSE-KMS**: Cifrado con claves gestionadas por cliente
- **S3 Object Lock**: Prevenir eliminación accidental
- **CloudTrail**: Registro de todas las llamadas API
- **Macie**: Descubrir datos sensibles automáticamente
- **Lambda Layers**: Código reutilizable seguro

#### Pasos de Implementación

1. **Crear S3 buckets** con cifrado SSE-KMS y políticas restrictivas
2. **Configurar KMS keys** con políticas de acceso específicas
3. **Crear IAM roles** para Lambda con permisos mínimos
4. **Desarrollar Lambda functions** para el pipeline
5. **Configurar VPC endpoints** para acceso privado a S3
6. **Habilitar CloudTrail** para auditoría
7. **Configurar CloudWatch** para monitoreo
8. **Implementar Macie** para detección de datos sensibles

---

### Proyecto 3: Ambiente Multi-Cuenta Seguro con Control Tower

#### Descripción del Proyecto
Implementar una estructura de múltiples cuentas AWS organizada y segura:
- Cuenta raíz (Root) - Solo para facturación
- Cuenta de Seguridad
- Cuenta de Logging/Auditoría
- Cuenta de Desarrollo
- Cuenta de Producción
- VPCs compartidas con segmentación

#### Arquitectura Sugerida

```
                            ┌─────────────────┐
                            │   AWS ROOT      │
                            │    ACCOUNT      │
                            │                 │
                            │  - Billing      │
                            │  - Organizations│
                            └────────┬────────┘
                                     │
              ┌──────────────────────┼──────────────────────┐
              │                      │                      │
              ▼                      ▼                      ▼
┌─────────────────────┐  ┌─────────────────────┐  ┌─────────────────────┐
│   SHARED SERVICES   │  │     SECURITY        │  │      LOGGING        │
│      ACCOUNT        │  │      ACCOUNT        │  │     ACCOUNT         │
│                     │  │                     │  │                     │
│ ┌─────────────────┐ │  │ ┌─────────────────┐ │  │ ┌─────────────────┐ │
│ │  Transit Gateway│ │  │ │   GuardDuty     │ │  │ │   CloudTrail    │ │
│ │  (Hub & Spoke)  │ │  │ │   Security Hub  │ │  │ │   Centralized   │ │
│ └─────────────────┘ │  │ │   Config        │ │  │ │   S3 Buckets    │ │
│                     │  │ └─────────────────┘ │  │ └─────────────────┘ │
│ ┌─────────────────┐ │  │                     │  │                     │
│ │  VPC Sharing    │  │  │                     │  │                     │
│ └─────────────────┘ │  │                     │  │                     │
└─────────────────────┘  └─────────────────────┘  └─────────────────────┘
         │                        │                        │
         │         ┌──────────────┼──────────────┐         │
         │         │              │              │         │
         ▼         ▼              ▼              ▼         ▼
┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐
│    DEV ACCOUNT   │  │  PROD ACCOUNT    │  │   TEST ACCOUNT  │
│                  │  │                  │  │                  │
│ ┌──────────────┐ │  │ ┌──────────────┐ │  │ ┌──────────────┐ │
│ │   Workloads  │ │  │ │  Workloads   │ │  │ │  Workloads   │ │
│ │   (Sandbox)  │ │  │ │  (Mission    │ │  │ │  (Testing)   │ │
│ │              │ │  │ │   Critical)  │ │  │ │              │ │
│ └──────────────┘ │  │ └──────────────┘ │  │ └──────────────┘ │
└──────────────────┘  └──────────────────┘  └──────────────────┘
```

#### Componentes de Seguridad a Implementar

| Componente | Configuración de Seguridad |
|------------|----------------------------|
| **AWS Organizations** | OU estructuradas (Root, Security, Prod, Dev) |
| **Service Control Policies (SCPs)** | Restringir servicios no deseados |
| **AWS Control Tower** | Landing Zone automatizada |
| **IAM Identity Center** | SSO centralizado |
| **Cross-Account Roles** | Acceso entre cuentas seguro |
| **VPC Sharing** | Recursos compartidos entre cuentas |
| **Transit Gateway** | Centralizar tráfico de red |

#### SCPs Recomendados

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "DenyAllRegionsExcept",
      "Effect": "Deny",
      "Action": "*",
      "Resource": "*",
      "Condition": {
        "StringNotEquals": {
          "aws:RequestedRegion": ["us-east-1", "us-west-2"]
        }
      }
    },
    {
      "Sid": "DenyDeleteCloudTrail",
      "Effect": "Deny",
      "Action": "cloudtrail:DeleteTrail",
      "Resource": "*"
    },
    {
      "Sid": "RequireS3Encryption",
      "Effect": "Deny",
      "Action": "s3:PutObject",
      "Resource": "arn:aws:s3:::*/*",
      "Condition": {
        "Bool": {
          "s3:x-amz-server-side-encryption": "false"
        }
      }
    }
  ]
}
```

#### Servicios de Seguridad Centralizados

- **Security Hub**: Vista consolidada de hallazgos de seguridad
- **GuardDuty**: Detección de amenazas
- **Config**: Auditoría de configuraciones
- **CloudTrail**: Registro de actividades
- **IAM Access Analyzer**: Análisis de acceso entre cuentas
- **Macie**: Protección de datos sensibles

#### Pasos de Implementación

1. **Crear Organization** en AWS Organizations
2. **Definir Organizational Units (OUs)** para cada ambiente
3. **Configurar SCPs** restrictivas a nivel de OU
4. **Configurar AWS Control Tower** para landing zone
5. **Crear cuentas** para cada ambiente
6. **Configurar IAM Identity Center** para SSO
7. **Implementar Transit Gateway** para conectividad
8. **Centralizar Logging** en cuenta de auditoría
9. **Configurar Security Hub** y GuardDuty
10. **Establecer Cross-Account Access** mediante roles

---

## Recursos Oficiales de AWS

- [AWS Certified Solutions Architect - Associate](https://aws.amazon.com/certification/certified-solutions-architect-associate/)
- [Exam Guide SAA-C03](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03.html)
- [Domain 1: Design Secure Architectures](https://docs.aws.amazon.com/aws-certification/latest/solutions-architect-associate-03/solutions-architect-associate-03-domain1.html)
- [AWS Well-Architected Framework - Security Pillar](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/wellarchitected-security-pillar.html)
- [AWS IAM Documentation](https://docs.aws.amazon.com/iam/)
- [Amazon VPC Documentation](https://docs.aws.amazon.com/vpc/)
- [AWS Security Documentation](https://docs.aws.amazon.com/security/)

---

*Documento basado en fuentes oficiales de AWS para el examen SAA-C03*
*Última actualización: 2026*
## API Report File for "graphql-transformer-core"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

/// <reference types="node" />

import { Condition } from 'cloudform-types/types/dataTypes';
import { ConditionIntrinsicFunction } from 'cloudform-types';
import { default as default_2 } from 'cloudform-types/types/dynamoDb/table';
import { default as default_3 } from 'cloudform-types/types/iam/role';
import { Diff as Diff_2 } from 'deep-diff';
import { DirectiveDefinitionNode } from 'graphql';
import { DirectiveNode } from 'graphql';
import { DocumentNode } from 'graphql';
import { EnumTypeDefinitionNode } from 'graphql';
import { EnumTypeExtensionNode } from 'graphql/language/ast';
import { EnumValueDefinitionNode } from 'graphql';
import { FieldDefinitionNode } from 'graphql';
import { GraphQLError } from 'graphql';
import { InputObjectTypeDefinitionNode } from 'graphql';
import { InputObjectTypeExtensionNode } from 'graphql/language/ast';
import { InputValueDefinitionNode } from 'graphql';
import { InterfaceTypeDefinitionNode } from 'graphql';
import { InterfaceTypeExtensionNode } from 'graphql/language/ast';
import { ObjectTypeDefinitionNode } from 'graphql';
import { ObjectTypeExtensionNode } from 'graphql';
import Output from 'cloudform-types/types/output';
import Parameter from 'cloudform-types/types/parameter';
import { Policy } from 'cloudform-types/types/iam/role';
import { Readable } from 'stream';
import Resource from 'cloudform-types/types/resource';
import { ScalarTypeDefinitionNode } from 'graphql';
import { SchemaDefinitionNode } from 'graphql';
import Template from 'cloudform-types/types/template';
import { Template as Template_2 } from 'cloudform-types';
import { TypeDefinitionNode } from 'graphql';
import { TypeSystemDefinitionNode } from 'graphql';
import { UnionTypeDefinitionNode } from 'graphql';
import { UnionTypeExtensionNode } from 'graphql/language/ast';

// Warning: (ae-forgotten-export) The symbol "ProjectOptions" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function buildAPIProject(opts: ProjectOptions): Promise<{
    resolvers: StringMap;
    stacks: {
        [name: string]: Template_2;
    };
    stackMapping: StackMapping_3;
    pipelineFunctions: StringMap;
    functions: {
        [path: string]: string;
    };
    schema: string;
    rootStack: Template_2;
}>;

// Warning: (ae-forgotten-export) The symbol "DiffableProject" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export const cantAddAndRemoveGSIAtSameTimeRule: (diff: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const cantBatchMutateGSIAtUpdateTimeRule: (diff: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const cantEditGSIKeySchemaRule: (diff: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// Warning: (ae-forgotten-export) The symbol "Diff" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export const cantHaveMoreThan500ResourcesRule: (diffs: Diff[], currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const cantMutateMultipleGSIAtUpdateTimeRule: (diffs: Diff[], currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const cantRemoveTableAfterCreation: (_: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const CLOUDFORMATION_FILE_NAME = "cloudformation-template.json";

// @public (undocumented)
export function collectDirectiveNames(sdl: string): string[];

// @public (undocumented)
export function collectDirectivesByType(sdl: string): Object;

// @public (undocumented)
export function collectDirectivesByTypeNames(sdl: string): {
    types: Object;
    directives: string[];
};

// @public (undocumented)
export type ConflictDetectionType = 'VERSION' | 'NONE';

// @public (undocumented)
export const enum ConflictHandlerType {
    // (undocumented)
    AUTOMERGE = "AUTOMERGE",
    // (undocumented)
    LAMBDA = "LAMBDA",
    // (undocumented)
    OPTIMISTIC = "OPTIMISTIC_CONCURRENCY"
}

// Warning: (ae-forgotten-export) The symbol "ResolversFunctionsAndSchema" needs to be exported by the entry point index.d.ts
// Warning: (ae-forgotten-export) The symbol "NestedStacks" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export interface DeploymentResources extends ResolversFunctionsAndSchema, NestedStacks {
    // (undocumented)
    stackMapping: StackMapping_3;
}

// @public (undocumented)
export class DestructiveMigrationError extends Error {
    constructor(message: string, removedModels: string[], replacedModels: string[]);
    // (undocumented)
    toString: () => string;
}

// @public (undocumented)
export type DiffRule = (diff: Diff, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export interface FeatureFlagProvider {
    // (undocumented)
    getBoolean(featureName: string, defaultValue?: boolean | null): boolean;
    // (undocumented)
    getNumber(featureName: string, defaultValue?: Number): Number;
    // (undocumented)
    getObject(featureName: string, defaultValue?: object): object;
}

// @public (undocumented)
export function getAppSyncServiceExtraDirectives(): string;

// @public (undocumented)
export const getCantAddLSILaterRule: (iterativeUpdatesEnabled?: boolean) => (diff: Diff_2<DiffableProject, DiffableProject>) => void;

// @public (undocumented)
export const getCantEditKeySchemaRule: (iterativeUpdatesEnabled?: boolean) => (diff: Diff_2<DiffableProject, DiffableProject>) => void;

// @public (undocumented)
export const getCantEditLSIKeySchemaRule: (iterativeUpdatesEnabled?: boolean) => (diff: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export const getCantRemoveLSILater: (iterativeUpdatesEnabled?: boolean) => (diff: Diff_2<DiffableProject, DiffableProject>, currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
export function getDirectiveArguments(directive: DirectiveNode): any;

// @public (undocumented)
export function getFieldArguments(type: any): any;

// @public (undocumented)
export function getSanityCheckRules(isNewAppSyncAPI: boolean, ff: FeatureFlagProvider, allowDestructiveUpdates?: boolean): {
    diffRules: DiffRule[];
    projectRules: ProjectRule[];
};

// @public (undocumented)
export function getTableNameForModel(sdl: string, modelName: string): string;

// @public (undocumented)
export function gql(literals: TemplateStringsArray, ...placeholders: string[]): DocumentNode;

// @public (undocumented)
export class GraphQLTransform {
    // Warning: (ae-forgotten-export) The symbol "GraphQLTransformOptions" needs to be exported by the entry point index.d.ts
    constructor(options: GraphQLTransformOptions);
    // (undocumented)
    transform(schema: string): DeploymentResources;
}

// @public (undocumented)
export class InvalidDirectiveError extends Error {
    constructor(message: string);
}

// @public (undocumented)
export class InvalidGSIMigrationError extends InvalidMigrationError {
    constructor(message: string, causedBy: string, fix: string);
    // (undocumented)
    causedBy: string;
    // (undocumented)
    fix: string;
}

// @public (undocumented)
export class InvalidMigrationError extends Error {
    constructor(message: string, causedBy: string, fix: string);
    // (undocumented)
    causedBy: string;
    // (undocumented)
    fix: string;
    // (undocumented)
    toString: () => string;
}

// @public (undocumented)
export class InvalidTransformerError extends Error {
    constructor(message: string);
}

// @public (undocumented)
export const isDataStoreEnabled: (projectDir: string) => Promise<boolean>;

// @public (undocumented)
export interface ITransformer {
    // (undocumented)
    after?: (acc: TransformerContext) => void;
    // (undocumented)
    argument?: (definition: InputValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    before?: (acc: TransformerContext) => void;
    // (undocumented)
    directive: DirectiveDefinitionNode;
    // (undocumented)
    enum?: (definition: EnumTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    enumValue?: (definition: EnumValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    field?: (parent: ObjectTypeDefinitionNode | InterfaceTypeDefinitionNode, definition: FieldDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    input?: (definition: InputObjectTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    inputValue?: (definition: InputValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    interface?: (definition: InterfaceTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    name: string;
    // (undocumented)
    object?: (definition: ObjectTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    scalar?: (definition: ScalarTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    typeDefinitions: TypeDefinitionNode[];
    // (undocumented)
    union?: (definition: UnionTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
}

// @public (undocumented)
function loadConfig(projectDir: string): Promise<TransformConfig>;
export { loadConfig }
export { loadConfig as readTransformerConfiguration }

// Warning: (ae-forgotten-export) The symbol "ProjectConfiguration" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
function loadProject(projectDirectory: string, opts?: ProjectOptions): Promise<ProjectConfiguration>;
export { loadProject }
export { loadProject as readProjectConfiguration }

// @public (undocumented)
export interface MappingParameters {
    // (undocumented)
    [key: string]: {
        [key: string]: {
            [key: string]: string | number | string[];
        };
    };
}

// Warning: (ae-forgotten-export) The symbol "MigrationOptions" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function migrateAPIProject(opts: MigrationOptions): Promise<{
    project: any;
    cloudBackend: any;
}>;

// @public (undocumented)
export const PARAMETERS_FILE_NAME = "parameters.json";

// @public (undocumented)
export type ProjectRule = (diffs: Diff[], currentBuild: DiffableProject, nextBuild: DiffableProject) => void;

// @public (undocumented)
function readSchema(projectDirectory: string): Promise<string>;
export { readSchema as readProjectSchema }
export { readSchema }

// @public (undocumented)
export type ResolverConfig = {
    project?: SyncConfig;
    models?: {
        [key: string]: SyncConfig;
    };
};

// Warning: (ae-forgotten-export) The symbol "AmplifyApiV1Project" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function revertAPIMigration(directory: string, oldProject: AmplifyApiV1Project): Promise<void>;

// @public (undocumented)
export const sanityCheckDiffs: (diffs: Diff[], current: DiffableProject, next: DiffableProject, diffRules: DiffRule[], projectRules: ProjectRule[]) => void;

// @public (undocumented)
export const sanityCheckProject: (currentCloudBackendDir: string, buildDirectory: string, rootStackName: string, diffRules: DiffRule[], projectRule: ProjectRule[]) => Promise<void>;

// @public (undocumented)
export class SchemaValidationError extends Error {
    constructor(errors: Readonly<GraphQLError[]>);
}

// @public (undocumented)
export function stripDirectives(doc: DocumentNode, except?: string[]): DocumentNode;

// @public (undocumented)
export type SyncConfig = SyncConfigOPTIMISTIC | SyncConfigSERVER | SyncConfigLAMBDA;

// @public (undocumented)
export type SyncConfigLAMBDA = {
    ConflictDetection: ConflictDetectionType;
    ConflictHandler: ConflictHandlerType.LAMBDA;
    LambdaConflictHandler: {
        name: string;
        region?: string;
        lambdaArn?: any;
    };
};

// @public (undocumented)
export type SyncConfigOPTIMISTIC = {
    ConflictDetection: ConflictDetectionType;
    ConflictHandler: ConflictHandlerType.OPTIMISTIC;
};

// @public (undocumented)
export type SyncConfigSERVER = {
    ConflictDetection: ConflictDetectionType;
    ConflictHandler: ConflictHandlerType.AUTOMERGE;
};

// @public (undocumented)
export module SyncUtils {
    // (undocumented)
    export function createSyncIAMRole(): default_3;
    // (undocumented)
    export function createSyncLambdaIAMPolicy({ name, region }: {
        name: string;
        region?: string;
    }): Policy;
    // (undocumented)
    export function createSyncTable(): default_2;
    // (undocumented)
    export function isLambdaSyncConfig(obj: any): obj is SyncConfigLAMBDA;
    // (undocumented)
    export function lambdaArnKey(name: string, region?: string): string;
    // Warning: (ae-forgotten-export) The symbol "DeltaSyncConfig" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    export function syncDataSourceConfig(): DeltaSyncConfig;
    // (undocumented)
    export function syncLambdaArnResource({ name, region }: {
        name: string;
        region?: string;
    }): ConditionIntrinsicFunction;
    // (undocumented)
    export function syncLambdaIAMRole({ name, region }: {
        name: string;
        region?: string;
    }): default_3;
    // Warning: (ae-forgotten-export) The symbol "SyncConfig_2" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    export function syncResolverConfig(syncConfig: SyncConfigOPTIMISTIC | SyncConfigLAMBDA | SyncConfigSERVER): SyncConfig_2;
    // (undocumented)
    export function syncTTLConfig(): {
        AttributeName: string;
        Enabled: boolean;
    };
}

// @public (undocumented)
export const TRANSFORM_BASE_VERSION = 4;

// @public (undocumented)
export const TRANSFORM_CONFIG_FILE_NAME = "transform.conf.json";

// @public (undocumented)
export const TRANSFORM_CURRENT_VERSION = 5;

// @public (undocumented)
export interface TransformConfig {
    // (undocumented)
    ElasticsearchWarning?: boolean;
    // (undocumented)
    Migration?: TransformMigrationConfig;
    // (undocumented)
    ResolverConfig?: ResolverConfig;
    // (undocumented)
    StackMapping?: {
        [resourceId: string]: string;
    };
    // (undocumented)
    TransformerOptions?: {
        [transformer: string]: {
            [option: string]: any;
        };
    };
    // (undocumented)
    transformers?: string[];
    // (undocumented)
    Version?: number;
    // (undocumented)
    warningESMessage?: boolean;
}

// @public (undocumented)
class Transformer_2 implements ITransformer {
    constructor(name: string, document: DocumentNode | string);
    // (undocumented)
    after?: (acc: TransformerContext) => void;
    // (undocumented)
    argument?: (definition: InputValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    before?: (acc: TransformerContext) => void;
    // (undocumented)
    directive: DirectiveDefinitionNode;
    // (undocumented)
    enum?: (definition: EnumTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    enumValue?: (definition: EnumValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    field?: (parent: ObjectTypeDefinitionNode | InterfaceTypeDefinitionNode, definition: FieldDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    input?: (definition: InputObjectTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    inputValue?: (definition: InputValueDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    interface?: (definition: InterfaceTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    name: string;
    // (undocumented)
    object?: (definition: ObjectTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    scalar?: (definition: ScalarTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
    // (undocumented)
    typeDefinitions: TypeDefinitionNode[];
    // (undocumented)
    union?: (definition: UnionTypeDefinitionNode, directive: DirectiveNode, acc: TransformerContext) => void;
}
export { Transformer_2 as Transformer }

// @public (undocumented)
export class TransformerContext {
    constructor(inputSDL: string, featureFlags: FeatureFlagProvider);
    // (undocumented)
    addEnum(en: EnumTypeDefinitionNode): void;
    // (undocumented)
    addEnumExtension(obj: EnumTypeExtensionNode): void;
    // (undocumented)
    addInput(inp: InputObjectTypeDefinitionNode): void;
    // (undocumented)
    addInputExtension(obj: InputObjectTypeExtensionNode): void;
    // (undocumented)
    addInterfaceExtension(obj: InterfaceTypeExtensionNode): void;
    // (undocumented)
    addMutationFields(fields: FieldDefinitionNode[]): void;
    // (undocumented)
    addObject(obj: ObjectTypeDefinitionNode): void;
    // (undocumented)
    addObjectExtension(obj: ObjectTypeExtensionNode): void;
    // (undocumented)
    addQueryFields(fields: FieldDefinitionNode[]): void;
    // (undocumented)
    addSubscriptionFields(fields: FieldDefinitionNode[]): void;
    // (undocumented)
    addType(obj: TypeDefinitionNode): void;
    // (undocumented)
    addUnionExtension(obj: UnionTypeExtensionNode): void;
    // (undocumented)
    readonly featureFlags: FeatureFlagProvider;
    // (undocumented)
    getMutation(): ObjectTypeDefinitionNode | undefined;
    // (undocumented)
    getMutationTypeName(): string | undefined;
    // (undocumented)
    getObject(name: string): ObjectTypeDefinitionNode | undefined;
    // (undocumented)
    getOutput(key: string): Output;
    // (undocumented)
    getQuery(): ObjectTypeDefinitionNode | undefined;
    // (undocumented)
    getQueryTypeName(): string | undefined;
    // (undocumented)
    getResolverConfig(): ResolverConfig;
    // (undocumented)
    getResource(resource: string): Resource;
    // (undocumented)
    getSchema(): SchemaDefinitionNode;
    // Warning: (ae-forgotten-export) The symbol "StackMapping" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    getStackMapping(): StackMapping;
    // (undocumented)
    getSubscription(): ObjectTypeDefinitionNode | undefined;
    // (undocumented)
    getSubscriptionTypeName(): string | undefined;
    // (undocumented)
    getTransformerVersion(): Number;
    // (undocumented)
    getType(name: string): TypeSystemDefinitionNode | undefined;
    // (undocumented)
    getTypeDefinitionsOfKind(kind: string): TypeDefinitionNode[];
    // (undocumented)
    inputDocument: DocumentNode;
    // (undocumented)
    isProjectUsingDataStore(): boolean;
    // (undocumented)
    mapResourceToStack(stackName: string, resource: string): void;
    // (undocumented)
    mergeConditions(conditions: {
        [key: string]: Condition;
    }): void;
    // (undocumented)
    mergeMappings(mapping: MappingParameters): void;
    // (undocumented)
    mergeOutputs(outputs: {
        [key: string]: Output;
    }): void;
    // (undocumented)
    mergeParameters(params: {
        [key: string]: Parameter;
    }): void;
    // (undocumented)
    mergeResources(resources: {
        [key: string]: Resource;
    }): void;
    // Warning: (ae-forgotten-export) The symbol "TransformerContextMetadata" needs to be exported by the entry point index.d.ts
    //
    // (undocumented)
    metadata: TransformerContextMetadata;
    // (undocumented)
    nodeMap: {
        [name: string]: TypeSystemDefinitionNode;
    };
    // (undocumented)
    putSchema(obj: SchemaDefinitionNode): void;
    // (undocumented)
    putType(obj: TypeDefinitionNode): void;
    // (undocumented)
    setOutput(key: string, output: Output): void;
    // (undocumented)
    setResolverConfig(resolverConfig: ResolverConfig): void;
    // (undocumented)
    setResource(key: string, resource: Resource): void;
    // (undocumented)
    setTransformerVersion(version: Number): void;
    // (undocumented)
    template: Template;
    // (undocumented)
    updateObject(obj: ObjectTypeDefinitionNode): void;
}

// @public (undocumented)
export class TransformerContractError extends Error {
    constructor(message: string);
}

// @public (undocumented)
export interface TransformMigrationConfig {
    // (undocumented)
    V1?: {
        Resources: string[];
    };
}

// @public (undocumented)
export class UnknownDirectiveError extends Error {
    constructor(message: string);
}

// Warning: (ae-forgotten-export) The symbol "UploadOptions" needs to be exported by the entry point index.d.ts
//
// @public (undocumented)
export function uploadAPIProject(opts: UploadOptions): Promise<void>;

// @public (undocumented)
function writeConfig(projectDir: string, config: TransformConfig): Promise<TransformConfig>;
export { writeConfig }
export { writeConfig as writeTransformerConfiguration }

// Warnings were encountered during analysis:
//
// src/util/amplifyUtils.ts:51:3 - (ae-forgotten-export) The symbol "StringMap" needs to be exported by the entry point index.d.ts
// src/util/amplifyUtils.ts:55:3 - (ae-forgotten-export) The symbol "StackMapping_3" needs to be exported by the entry point index.d.ts

// (No @packageDocumentation comment for this package)

```
